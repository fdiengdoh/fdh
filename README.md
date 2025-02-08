# My Own Link List app

This is a Link List webapp similar to linktree. The Link List include the following sections
- Profile Picture or Logo
- Profile name
- Links

How this app was created?
This app is created in local environment using PHP and I have used [Bootstrap](https://getbootstrap.com/) for styling with a few minor adjustment to my taste. I also use bootstrap icon and just include those via cdn. To add new links edit the file [link.php](link.php) and add new links to this section below: 

```
<?php
  $links = [
      //Add New Link on this line using this format [ 'link' => 'link-url-here', 'icon' => 'bootstrap-icon here', 'title' => 'Title of the Link' ]
      [ 'link' => 'https://www.fdiengdoh.com/2023/01/calendar-2023.html', 'icon' => '<i class="bi bi-link-45deg"></i>', 'title' => 'Ka Kyrteng jong ki Bnai ha ka Ktien Khasi' ],
      [ 'link' => 'https://www.fdiengdoh.com/2022/04/useful-email-aliases-using-google-mail.html', 'icon' => '<i class="bi bi-link-45deg"></i>', 'title' => 'Useful Email Aliases using GMail' ],
      [ 'link' => 'https://www.fdiengdoh.com/2020/07/ka-ei-ka-vaccine.html', 'icon' => '<i class="bi bi-link-45deg"></i>', 'title' => 'Ka ei ka Baksin (Vaccine)?' ],
      [ 'link' => 'https://youtu.be/tTNKS6CsG3o', 'icon' => '<i class="bi bi-camera-video-fill"></i>', 'title' => 'Ka Hima Lyngiong' ],
      [ 'link' => 'https://youtu.be/fix8QC_rlY8', 'icon' => '<i class="bi bi-camera-video-fill"></i>', 'title' => 'Resonate Router UPS: A Review'],
      [ 'link' => 'https://youtu.be/RRSOQHD1H50', 'icon' => '<i class="bi bi-camera-video-fill"></i>', 'title' => "Meghalaya - a bird's eye view"],
      [ 'link' => 'https://youtu.be/GmoQa8Y61TE', 'icon' => '<i class="bi bi-camera-video-fill"></i>', 'title' => "Phe Phe Falls - Jaiñtia Hills"],
      [ 'link' => 'https://www.youtube.com/playlist?list=PLnAxMOVwqslFysqxWXNin2Y2w5J2y17Od', 'icon' => '<i class="bi bi-camera-video-fill"></i>', 'title' => "Travel - Vlogs"],
      [ 'link' => 'https://www.youtube.com/playlist?list=PLnAxMOVwqslEjju22ao-CcfceynfUpVXt', 'icon' => '<i class="bi bi-camera-video-fill"></i>', 'title' => "Unboxing - Tutorials"],
  ];
?>
```

The link is in this format

```
[ 'link' => 'link-url-here', 'icon' => 'bootstrap-icon here', 'title' => 'Title of the Link' ]
```

The above [link.php](file) is then converted to html file using a simple command in linux as follows

```
php /location/of/your/link.php > index.html
```

The generated index.html file is then uploaded to a public server that can be hosted as a github page too. 

My app is [here](https://fdh.pw)
