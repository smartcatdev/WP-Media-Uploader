
Create a media upload button button to use in your WordPress plugins or themes. 

Features :
- Easy to setup and use
- Customizable : Make this work for your needs
- Tiny ( less than 3 KB )

## Version
1.0

## License

## Basic usage
1. HTML
```` HTML
<div class="form-group smartcat-uploader">
    <label for="logo">Company logo</label>
    <input type="text" name="logo">
</div>
````

2. PHP
```` PHP
// This will load the required dependencies for the WordPress media uploader
function load_admin_libs() {
    wp_enqueue_media();
}
add_action( 'admin_enqueue_scripts', 'load_admin_libs' );
````

3. JavaScript
```` javascript
$.wpMediaUploader();
````

## Advanced usage
```` javascript
$.wpMediaUploader({

    target : '.smartcat-uploader', // The class wrapping the textbox
    uploaderTitle : 'Select or upload image', // The title of the media upload popup
    uploaderButton : 'Set image', // the text of the button in the media upload popup
    multiple : false, // Allow the user to select multiple images
    buttonText : 'Upload image', // The text of the upload button
    buttonClass : '.smartcat-upload', // the class of the upload button
    previewSize : '150px', // The preview image size
    modal : false, // is the upload button within a bootstrap modal ?
    buttonStyle : { // style the button
        color : '#fff',
        background : '#3bafda',
        fontSize : '16px',                
        padding : '10px 15px',                
    },

});
````

## Preview
[preview]: preview.jpg "Standard appearance"