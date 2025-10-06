<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Travel</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css" integrity="sha512-2SwdPD6INVrV/lHTZbO2nodKhrnDdJK9/kg2XD1r9uGqPo1cUbujc+IYdlYdEErWNu69gVcYgdxlmVmzTWnetw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
   
    <style>
        .navbar {
            display: flex;
            background-color: lightgray;
            padding: 10px 10px;
            justify-content: space-evenly;
            align-items: left;
            box-shadow: 0 2px 4px gray;
            color: black;
            text-decoration: none;
            overflow: hidden;
        }
        .navbar a:hover {
            background-color: lightblue;
            color: black;
            padding: 5px;
            border-radius: 3px; 
            
        }
         .nav-links a {
      color: white;
      text-decoration: none;
      margin-left: 15px;
    }
    .menu-btn{
      align-items: left;
    }

    /* Desktop: show links */
    @media (min-width: 768px) {
      .menu-btn { display: none; }
      .nav-links { display: block; }
    }

    /* Mobile: hide links, show menu button */
    @media (max-width: 767px) {
      .menu-btn { display: block; cursor: pointer; }
      .nav-links { display: none; flex-direction: column; margin-top: 10px; }
      .nav-links.show { display: flex; }
      .nav-links a { margin: 10px 0; }
    
    }
        .content {
            padding: 10px;
            text-align: center;
            
        }
         h1 {
            font-size: 40px;

            margin-bottom: 10px;
            background-color: lightblue;
            border: 2px solid black; 
            padding: 100px;
            border-radius: 10px;
            text-align: center;
            color: azure;
            animation-name: myAnimation;
            animation-duration: 6s;
            animation-iteration-count: infinite;
            /* background-repeat: no-repeat;
            background-position: center; */
            
            
        } 
      
        @keyframes myAnimation {
         from {background-image: url(https://external-preview.redd.it/nEjl5B2gCpXaXjqLNiwc_Q47LF4toKbYaGKadOkvBWk.jpg?width=640&crop=smart&auto=webp&s=736bd0b2496ead520e47180f5074de85f08adbef);}
         to {background-image:url(https://www.shutterstock.com/image-photo/taj-mahal-main-view-on-260nw-2378053017.jpg);}
}
        label{
            font-size: 20px;
        }  
    
        /* img {
              width: 500px;
              height: 400px;
              min-width: 50; 
              max-width: 600px;
              margin: 0 auto;
              display: flex;
        } 

            @media (max-width: 500px) {
        img {
            max-width: 100%;
            min-width: 50px;
            }
        }  */

     img {
  max-width: 100%;
  height: auto;
  display: block;
  margin: 0 auto;
}
    /* .search-box {
      width: 120px;
      max-width: 60vw;
      padding: 3px;
      border-radius: 20px;
      border: 1px solid pink;
      outline: none;
      margin:2px;
    }
    .search-btn {
      padding: 5px 5px;
      border: none;
      border-radius: 20px;
      background-color: #4CAF50;
      color: white;
      cursor: pointer;
      width: 50px;
    } */
       .search-box {
      width: 250px;
      padding: 4px;
      border-radius: 20px;
      border: 1px solid pink;
      outline: none;
    }
    .search-btn {
      padding: 8px 8px;
      border: none;
      border-radius: 20px;
      background-color: #4CAF50;
      color: white;
      cursor: pointer;
    }
    .search-btn:hover {
      background-color: #45a049;
    }
    h3 {
        text-align: center;
    }
    select {
        padding: px;
        border-radius: px;
        border: 1px solid lightcoral;
        outline: none;
        background-color: pink;
        size-adjust: 5px;
        font-size: 10px;
    }
    .content{
        background-color: black;
        color: white;
        padding: 40px;
        margin: 20px;
       
        } 
       
    body{
         animation-name: aNnimation;
        animation-duration: 8s;
        animation-iteration-count: infinite;
        width: auto;

        }

         @keyframes aNnimation {
         from {background-color:lightyellow;}
         to {background-color:lightcyan;}
}
.animated-bg {
  width: 90vw;
  max-width: 600px;
  height: 300px;
  margin: 40px auto;
  border-radius: 16px;
  box-shadow: 0 4px 16px rgba(0,0,0,0.12);
  background-size: cover;
  background-position: center;
  animation: imageSlide 12s infinite;
}

/* 3-image animation */
@keyframes imageSlide {
  0%   { background-image: url('https://dynamic-media-cdn.tripadvisor.com/media/photo-o/24/ae/c7/8c/caption.jpg?w=600&h=600&s=1'); }
  33%  { background-image: url('https://upload.wikimedia.org/wikipedia/commons/5/56/Mysuru_Montage.jpg'); }
  66%  { background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSv-vOEiKId8BGkFJBqWzcduFRM9BNPl0dEKA&s'); }
  100% { background-image: url('https://dynamic-media-cdn.tripadvisor.com/media/photo-o/24/ae/c7/8c/caption.jpg?w=600&h=600&s=1'); }
}
  
    </style>
</head>
<body>
    <div class ="navbar">
    <div class="menu-btn">☰</div>
    <div class="nav-links">
        <a href="#home">Home</a>
        <a href="#about">About </a>
        <a href="Privacy.html">Privacy policy</a>
        <a href="login.html">Login</a>
    </div>

    <form action="https://www.google.com/search" method="get">
    <input type="text" name="q" class="search-box" placeholder="Search...">
    <button type="submit" class="search-btn"><i class="fa fa-search"></i></button>

</form>
</div>

    
        <h1 style="font-size: 5vw; background-image: url(https://external-preview.redd.it/nEjl5B2gCpXaXjqLNiwc_Q47LF4toKbYaGKadOkvBWk.jpg?width=640&crop=smart&auto=webp&s=736bd0b2496ead520e47180f5074de85f08adbef)">Welcome To Our World</h1>
    <p>
        <h3 style="font-size: 4vw;">✨ Welcome to the Land of Wonders– India!✨</h3>
            India is not just a country, it’s an experience. From the snow-capped Himalayas to the golden deserts of Rajasthan, from the serene backwaters of Kerala to the bustling streets of Delhi and Mumbai – every corner tells a story. With its rich culture, ancient history, vibrant traditions, and breathtaking landscapes, India is truly a traveler’s paradise.
            Whether you seek spirituality, adventure, heritage, or modern city life, India offers a perfect blend of the old and the new. Join us as we explore the best places in India that capture the heart and soul of this incredible nation. 🌏❤️</p>
        
        <h3><span style="background-color: #45a049; font-size: 4dvw;">🌟 Top 10 Best Places to Visit in India</span></h3>

        <h2 >1. Taj Mahal, Agra</h2>
        <div class="animated-bg"></div>

           <p style="text-align: center;"> The Taj Mahal is one of the most famous monuments in the world and a symbol of love, beauty, and architectural brilliance. 🌸<br>
            The Taj Mahal, located in Agra, Uttar Pradesh, is one of the most iconic monuments in the world and a symbol of eternal love. Built by the Mughal emperor Shah Jahan in memory of his beloved wife Mumtaz Mahal, it took about 22 years to complete, from 1632 to 1653. This breathtaking mausoleum is constructed from white marble that reflects different shades with the changing light of the sun and moon,
             making it appear magical at every hour of the day. The Taj Mahal is surrounded by beautifully designed gardens, fountains, and a reflecting pool that enhances its beauty. Recognized as a UNESCO World Heritage Site, it is admired globally as one of the finest examples of Mughal architecture, blending Persian, Islamic, and Indian styles. Beyond its architectural brilliance, the Taj Mahal stands as a timeless symbol of love, devotion, and artistic excellence. <br><br>
        <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/24/ae/c7/8c/caption.jpg?w=600&h=600&s=1" height="500px">
</p>
        <h2>2. Jaipur, Rajasthan</h2>
        <div class="animated-ab"></div>

        <p style="text-align: center;"> Known as the "Pink City" for its distinctive pink-colored buildings, Jaipur is a vibrant city that offers a rich blend of history, culture, and architecture. 🌆<br>
            Jaipur, the capital city of Rajasthan, is famously known as the "Pink City" due to the distinct pink hue of its buildings in the old city area. This vibrant city is a treasure trove of history, culture, and architectural marvels. Founded in 1727 by Maharaja Sawai Jai Singh II, Jaipur is renowned for its majestic forts, palaces, and 
            bustling bazaars. Key attractions include the Amber Fort, City Palace, Hawa Mahal (Palace of Winds), and Jantar Mantar, an astronomical observatory. The city's rich cultural heritage is reflected in its traditional arts and crafts, colorful festivals, and delectable Rajasthani cuisine. Jaipur's blend of royal history and modern vibrancy makes it a must-visit destination for travelers seeking an authentic Indian experience. <br>
        <img src="data:image/jpeg;base64,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" alt="jaipur"> <br>
        <img src="data:image/jpeg;base64,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" alt="">
    <h2>3. Varanasi, Uttar Pradesh</h2>

    <p style="text-align: center;">Known as the spiritual capital of India, Varanasi is one of the oldest continuously inhabited cities in the world. It is famous for its ghats along the Ganges River, where pilgrims perform rituals and ceremonies. The city is also renowned for its silk weaving and vibrant cultural heritage.</p>
          <img src="https://bespokeindiatravel.co.uk/wp-content/uploads/2017/12/Varanasi-Uttar-Pradesh.jpg" alt="">
    <h2>4. Goa</h2>

    <p style="text-align: center;">Goa is a popular beach destination known for its stunning coastline, vibrant nightlife, and Portuguese heritage. It offers a mix of beautiful beaches, historic churches, and lively markets. Goa is also famous for its seafood cuisine and annual music festivals.</p>
           <img src="https://goadarling.com/wp-content/uploads/2023/10/best-selling-goa-trip-package-for-friends-4-days-3-nights.png" alt="">
    <h2>5.Leh-Ladakh (Jammu & Kashmir)</h2>

    <p style="text-align: center;">Leh-Ladakh is a high-altitude desert region known for its breathtaking landscapes, including rugged mountains, serene lakes, and ancient monasteries. It is a haven for adventure enthusiasts, offering activities like trekking, river rafting, and mountain biking. The region's unique culture and stunning vistas make it a must-visit destination.</p>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT1KSA9AnwbQj3bX4YWOugRmw7LUPARZSczXA&s" alt="leh=ladakh">
    <h2>6. Darjeeling (West Bengal)</h2>

    <p style="text-align: center;">Darjeeling is a charming hill station known for its tea plantations, panoramic views of the Himalayas, and colonial architecture. The town offers a cool climate, scenic train rides on the Darjeeling Himalayan Railway, and opportunities for trekking and exploring nearby monasteries. Darjeeling's unique blend of natural beauty and cultural heritage makes it a popular destination.</p>
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSFlVpJvpNPhot6l_8kQwB6Jhd3APZ3XbDxTQ&s" alt="">
     
<h2>7. Mysore (Karnataka)</h2>

    <p style="text-align: center;">Mysore is known for its rich history, grand palaces, and vibrant cultural scene. The city is famous for the Mysore Palace, a stunning example of Indo-Saracenic architecture, and the annual Dasara festival, which showcases traditional music, dance, and processions. Mysore is also renowned for its silk sarees and sandalwood products.</p>
    <img src="https://upload.wikimedia.org/wikipedia/commons/5/56/Mysuru_Montage.jpg" alt="">
    
    <h2>8. Rishikesh (Uttarakhand)</h2>

    <p style="text-align: center;">Rishikesh is a spiritual and adventure hub located on the banks of the Ganges River. It is known for its yoga and meditation centers, attracting seekers from around the world. Rishikesh also offers thrilling activities like white-water rafting, trekking, and camping. The town's serene environment and spiritual ambiance make it a popular destination for relaxation and self-discovery.</p>
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcStFz1HLpKGzXnrtvj28FW5xzU0sqvORjQ3_w&s" alt="">

<h2>9.Delhi</h2>

<p style="text-align: center;">Delhi, the capital city of India, is a bustling metropolis that seamlessly blends history and modernity. It is home to iconic landmarks such as the Red Fort, Qutub Minar, and India Gate. Delhi offers a rich cultural experience with its diverse cuisine, vibrant markets, and historical sites. The city is also a gateway to exploring other parts of India.</p>
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ_vxm9haE9GZnu75y8LnCno_nQ9P59OGRdlA&s" alt="">

<h2>10.Kerala (Backwaters & Munnar)</h2>

<p style="text-align: center;">Kerala, often referred to as "God's Own Country," is known for its picturesque backwaters, lush greenery, and serene hill stations like Munnar. The backwaters offer a unique experience of cruising through interconnected canals, lakes, and lagoons, while Munnar is famous for its tea plantations and cool climate. Kerala is also renowned for its Ayurvedic treatments, vibrant festivals, and rich cultural heritage.</p>
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSv-vOEiKId8BGkFJBqWzcduFRM9BNPl0dEKA&s" alt=""> <br>


<p>✨ India is a land of incredible diversity, where every destination tells its own story through culture, history, and natural beauty. From the timeless elegance of the Taj Mahal to the serene backwaters of Kerala, the vibrant cities of Jaipur and Delhi, and the breathtaking landscapes of Leh-Ladakh, these top 10 places capture the essence of India’s charm.
    Whether you seek adventure, spirituality, relaxation, or heritage, India promises unforgettable experiences at every corner. Start planning your journey and explore the magic that makes India truly extraordinary!</p> <br>
<h2>11.Noida</h2>
<div class="animated-bg"></div>
     
<div class="content">
   <p>Thank you for visiting our website! We appreciate your time and interest.</p>
    <p>Contact us:</p>
    <a href="https://www.facebook.com/"> <i class="fa-brands fa-facebook" style="color: blue;"></i></a>
    <a href="https://www.Instagram.com"><i class="fa-brands fa-instagram" style="color: purple;"></i></a>
    <a href="https://www.twitter.com"><i class="fa-brands fa-twitter" style="color:lightseagreen"></i></a>
</div>
<script>
    const menuBtn = document.querySelector('.menu-btn');
    const navLinks = document.querySelector('.nav-links');

    menuBtn.onclick = () => {
      navLinks.classList.toggle('show');
    };
    </script>
</body> 
</html>
