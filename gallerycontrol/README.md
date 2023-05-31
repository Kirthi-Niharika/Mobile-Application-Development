# Ex.No:8 To create a gallery control using android studio to display images or photos.


## AIM:

To create a gallery control using android studio to display images or photos.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Studio and then click on File -> New -> New project.
Step 2: Then type the Application name as HelloWorld and click Next. 
Step 3: Then select the Minimum SDK as shown below and click Next.
Step 4: Then select the Empty Activity and click Next. Finally click Finish.
Step 5: Design layout in activity_main.xml.
Step 6: Display message give in MainActivity file.
Step 7: Save and run the application.



## PROGRAM:
```
/*
Program to print the text “GalleryControl”.
Developed by:T.Kirthi Niharika
Registeration Number :212221040084
*/
```
activity_main.xml

Design a simple application to display/play the video in android activity or view using raw 
folder. 
MainActivity.java

package com.example.gallery;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Gallery;
import android.view.View;
import android.widget.AdapterView;
import android.widget.Gallery;
import android.widget.ImageView;
public class MainActivity extends AppCompatActivity {
    Gallery simpleGallery;
    // CustomizedGalleryAdapter is a java class which extends BaseAdapter
// and implement the override methods.
    CustomizedGalleryAdapter customGalleryAdapter;
    ImageView selectedImageView;
    // To show the selected language, we need this
// array of images, here taken 10 different kind of most popular programming languages
    int[] images = {R.drawable.img, R.drawable.img_1,R.drawable.img_2,R.drawable.img_3,R.drawable.img_4};
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
// Our layout is activity_main
// get the reference of Gallery. As we are showing languages it is named as languagesGallery
// meaningful names will be good for easier understanding
        simpleGallery = (Gallery) findViewById(R.id.languagesGallery);
// get the reference of ImageView
        selectedImageView = (ImageView) findViewById(R.id.imageView);
// initialize the adapter
        customGalleryAdapter = new CustomizedGalleryAdapter(getApplicationContext(), images);
// set the adapter for gallery
        simpleGallery.setAdapter(customGalleryAdapter);
// Let us do item click of gallery and image can be identified by its position
        simpleGallery.setOnItemClickListener(new AdapterView.OnItemClickListener() {
            @Override
            public void onItemClick(AdapterView<?> parent, View view, int position, long id) {
// Whichever image is clicked, that is set in the selectedImageView
// position will indicate the location of image
                selectedImageView.setImageResource(images[position]);
            }
        });
    }
}


CustomizedGalleryAdapter.java

package com.example.gallery;
import android.content.Context;
import android.view.View;
import android.view.ViewGroup;
import android.widget.BaseAdapter;
import android.widget.Gallery;
import android.widget.ImageView;
public class CustomizedGalleryAdapter extends BaseAdapter {
    private Context context;
    private int[] images;
    public CustomizedGalleryAdapter(Context c, int[] images) {
        context = c;
        this.images = images;
    }
    // returns the number of images, in our example it is 10
    public int getCount() {
        return images.length;
    }
    // returns the Item of an item, i.e. for our example we can get the image
    public Object getItem(int position) {
        return position;
    }
    // returns the ID of an item
    public long getItemId(int position) {
        return position;
    }
    // returns an ImageView view
    public View getView(int position, View convertView, ViewGroup parent) {
// position argument will indicate the location of image
// create a ImageView programmatically
        ImageView imageView = new ImageView(context);
// set image in ImageView
        imageView.setImageResource(images[position]);
// set ImageView param
        imageView.setLayoutParams(new Gallery.LayoutParams(200, 200));
        return imageView;
    }
}


## OUTPUT

<img width="910" alt="Screenshot 2023-05-31 214831" src="https://github.com/Kirthi-Niharika/Mobile-Application-Development/assets/114135005/f8f04a05-ea07-4b69-a699-dff288ddf5c5">
<img width="182" alt="Screenshot 2023-05-31 214859" src="https://github.com/Kirthi-Niharika/Mobile-Application-Development/assets/114135005/0e133611-334d-4331-9a61-5a6da415bf88">



## RESULT
Thus a Simple Android Application to create a gallery control using android studio to display images or photos is developed and executed successfully.


