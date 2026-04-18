# My Own Link List app

This is a Link List webapp similar to linktree. The Link List include the following sections
- Profile Picture or Logo
- Profile name
- Links

How this app was created?
This app is created in local environment using PHP and I have used a simple custom css for styling with selected icons from [fontawesome icons](https://fontawesome.com/icons) as svg sprite to reduce size. To add new links edit the file [link.php](link.php) and add new links to this section below: 

```
<?php
  $links = [
    //Add New Link on this line using this format [ 'link' => 'link-url-here', 'icon' => 'icon here', 'title' => 'Title of the Link' ]
      [ 'link' => 'https://www.fdiengdoh.com/2025/02/link-list-for-my-social-media.html', 'icon' => 'link-icon', 'title' => 'My Own Social Media Link List' ],
      [ 'link' => 'https://www.fdiengdoh.com/2023/01/calendar-2023.html', 'icon' => 'link-icon', 'title' => 'Ka Kyrteng jong ki Bnai ha ka Ktien Khasi' ],
      [ 'link' => 'https://www.fdiengdoh.com/2022/04/useful-email-aliases-using-google-mail.html', 'icon' => 'link-icon', 'title' => 'Useful Email Aliases using GMail' ],
      [ 'link' => 'https://www.fdiengdoh.com/2020/07/ka-ei-ka-vaccine.html', 'icon' => 'link-icon', 'title' => 'Ka ei ka Baksin (Vaccine)?' ],
      [ 'link' => 'https://youtu.be/tTNKS6CsG3o', 'icon' => 'video-icon', 'title' => 'Ka Hima Lyngiong' ],
      [ 'link' => 'https://youtu.be/fix8QC_rlY8', 'icon' => 'video-icon', 'title' => 'Resonate Router UPS: A Review'],
      [ 'link' => 'https://youtu.be/RRSOQHD1H50', 'icon' => 'video-icon', 'title' => "Meghalaya - a bird's eye view"],
      [ 'link' => 'https://youtu.be/GmoQa8Y61TE', 'icon' => 'video-icon', 'title' => "Phe Phe Falls - Jaiñtia Hills"],
      [ 'link' => 'https://www.youtube.com/playlist?list=PLnAxMOVwqslFysqxWXNin2Y2w5J2y17Od', 'icon' => 'video-icon', 'title' => "Travel - Vlogs"],
      [ 'link' => 'https://www.youtube.com/playlist?list=PLnAxMOVwqslEjju22ao-CcfceynfUpVXt', 'icon' => 'video-icon', 'title' => "Unboxing - Tutorials"],
  ];
?>
```

The link is in this format

```
[ 'link' => 'link-url-here', 'icon' => 'icon here', 'title' => 'Title of the Link' ]
```

The above [file](link.php) is then converted to html file using a simple command in linux as follows

```
php /location/of/your/link.php > index.html
```

The generated index.html file is then uploaded to a public server that can be hosted as a github page too. 

My app is [here](https://fdh.pw)
