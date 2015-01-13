DSAvataImageView
================
Subclass of ImageView to create a circle avatar image view with user name initial image view.

![screenshot](https://cloud.githubusercontent.com/assets/7636468/5624104/0bf3d9f8-95a3-11e4-99f3-92afa3fb7efe.png)

Usage
--------

###XML (Use Circle avatar image view)
```xml
    <com.xperi.avataimageview.DSAvatarImageView
        android:layout_width="250dp"
        android:layout_height="250dp"
        android:src="@drawable/image"
        app:border_color="#EEEEEE"
        app:border_width="5dp"
        />
```
###XML (Use user name initial view) output 'SJ'
```xml
    <com.xperi.avataimageview.DSAvatarImageView
        android:layout_width="250dp"
        android:layout_height="250dp"
        app:border_color="#EEEEEE"
        app:border_width="5dp"
        app:name="steve jobs"
        app:background_color="@android:color/white"
		app:text_color="@android:color/black"
        />
```
You may use the following properties in your XML to customize your DSAvataImageView.

#####Properties:

* `app:border`              (boolean)           -> default true
* `app:border_color`        (color)             -> default GRAY
* `app:border_width`        (dimension)         -> default 2dp
* `app:name`                (String)            -> default 
* `app:background_color`    (color)             -> default WHITE
* `app:text_color`          (color)             -> default GRAY
###JAVA (Use Circle avatar image view)

```java
    DSAvatarImageView avataImageView=getView(convertView, R.id.circularIv);
    avataImageView.setBorderColor(getResources().getColor(R.color.GrayLight));
    avataImageView.setBorderWidth(10);
    avataImageView.setImageResource(R.id.sample);
```
###JAVA (Use user name initial view) output 'SJ'

```java
    DSAvatarImageView avataImageView=getView(convertView, R.id.circularIv);
    avataImageView.setBorderColor(getResources().getColor(R.color.GrayLight));
    avataImageView.setName("steve jobs")
```
