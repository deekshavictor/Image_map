# Ex04 Places Around Me
# Date: 01/12/2025
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
{% load static %}
<html>
<head>
    <title>NAMMA ERODE</title>
    <style>
        img {
            width: 100%;
            height: auto;   
        }
        body {
            overflow: hidden;
            font-family: Arial;
        }
    </style>
</head>

<body>
    <h1>ERODE CITY</h1>
    <h2>DEEKSHA VICTOR SELVAKUMAR SINDHUPRIYA (25018981)</h2>

    <img src="{% static 'erode map.png' %}" alt="Erode" usemap="#image-map">

    <map name="image-map">
        <area shape="rect" coords="953,347,1122,384" href="{% url 'park' %}"   title="Barriage Park">
        <area shape="rect" coords="576,111,694,162" href="{% url 'sant' %}"   title="Bird Sanctuary">
        <area shape="rect" coords="1152,547,1289,616" href="{% url 'temple' %}"   title="Nattatreeswarar Temple">
        <area shape="rect" coords="650,401,751,445" href="{% url 'thindal' %}"   title="Thindal">
        
    </map>

</body>
</html>
park.html
{% load static %}
<!DOCTYPE html>
<html>
<head>
    <title>Odapalli Barrage Park</title>
    <style>
        body {
            background: #e8f5e9; /* light green background */
            font-family: "Georgia", serif;
            color: #9258c8; /* deep green text */
            margin: 0;
            padding: 0;
        }
        h1 {
            text-align: center;
            color: #73529c; /* darker green for heading */
            padding: 25px;
            font-size: 2.5em;
            border-bottom: 3px solid #a36ee0; /* decorative underline */
        }
        img {
            display: block;
            margin: 30px auto;
            width: 75%; /* responsive width */
            max-width: 800px;
            height: auto;
            border-radius: 20px;
            border: 4px solid #be65d0; /* green border */
        }
        p {
            text-align: justify;
            line-height: 1.9;
            padding: 25px 60px;
            font-size: 17px;
            background-color: #ffffff;
            border-radius: 12px;
            margin: 30px auto;
            max-width: 950px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        }
    </style>
</head>
<body>
    <h1>Odapalli Barrage Park</h1>
    <img src="{% static 'park.jpg'%}" alt="Odapalli Barrage Park">
    <p>
        Odapalli Barrage Park is a popular recreational spot in Pallipalayam, near Erode, Tamil Nadu, known for its scenic beauty and peaceful atmosphere.
        Situated along the Erode–Kokkarayanpettai Road, the park is built around the Odapalli Barrage, making it a unique blend of nature and engineering.
        It serves as a favorite hangout for families, children, and tourists who come to enjoy the lush greenery, fresh air, and the calming view of water flowing through the barrage.
        The park is open daily from 7:00 AM to 6:00 PM, making it an accessible destination for morning walks, picnics, and evening relaxation.
        Its proximity—just about 3 kilometers from Erode Junction railway station—adds to its convenience for visitors.
        With well-maintained pathways, seating areas, and a serene riverside environment, Odapalli Barrage Park has become a local landmark for leisure and tourism.
        The gentle flow of water, combined with the landscaped surroundings, creates a refreshing escape from the bustle of city life.
        In essence, Odapalli Barrage Park is more than just a park—it is a community space that connects people with nature, offering relaxation, scenic views, and a touch of tranquility right at the edge of Erode city.
    </p>
</body>
</html>
sant.html
{% load static %}
<!DOCTYPE html>
<html>
<head>
    <title>Bird Sanctuary</title>
    <style>
        body {
            background: #e3f2fd; /* soft blue background */
            font-family: "Helvetica Neue", Arial, sans-serif;
            color: #0d47a1; /* deep blue text */
            margin: 0;
            padding: 0;
        }
        h1 {
            text-align: center;
            color: #1565c0; /* bold blue heading */
            padding: 30px;
            font-size: 3em;
            text-transform: uppercase;
            letter-spacing: 3px;
            border-bottom: 4px solid #64b5f6; /* stylish underline */
        }
        img {
            display: block;
            margin: 25px auto;
            width: 85%; /* responsive width */
            max-width: 900px;
            height: auto;
            border-radius: 15px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.3); /* strong shadow */
            transition: transform 0.4s ease-in-out;
        }
        img:hover {
            transform: scale(1.07); /* zoom effect */
        }
        p {
            text-align: justify;
            line-height: 2;
            padding: 35px 60px;
            font-size: 18px;
            background-color: #ffffff;
            border-radius: 15px;
            margin: 40px auto;
            max-width: 1000px;
            box-shadow: 0 6px 14px rgba(0,0,0,0.2);
            color: #333; /* softer text for readability */
        }
    </style>
</head>
<body>
    <h1>Chithode Bird Sanctuary</h1>
    <img src="{%static 'bird.jpg'%}" alt="Bird Sanctuary">
    <p>
        Chithode Bird Sanctuary, located near Erode in Tamil Nadu, is a serene haven for migratory and native birds.
        This sanctuary is often associated with the Vellode Bird Sanctuary, which lies close to Chithode and is one of the most important protected areas in the Kongu region.
        Spread around a large lake, the sanctuary provides a safe habitat for thousands of birds that arrive from different parts of the world.
        Species such as cormorants, teals, pintail ducks, pelicans, and darters are commonly sighted here, making it a paradise for bird watchers and nature enthusiasts.
        Established in 1996 by the Ministry of Environment and Forests, the sanctuary is part of Tamil Nadu’s official list of protected areas.
        Its centerpiece is the Periyakulam Lake, which attracts birds due to its abundant water and food resources.
        Unlike other sanctuaries surrounded by dense forests, Chithode–Vellode Bird Sanctuary is unique because it is built around a water tank, giving visitors clear views of the birds in their natural setting.
        The sanctuary plays a vital role in conservation and ecological balance, offering shelter to migratory species during winter and supporting local biodiversity year-round.
        For visitors, it is not only a place to observe birds but also a peaceful escape into nature, away from the bustle of Erode city.
        In essence, Chithode Bird Sanctuary stands as a living classroom of ecology, blending scenic beauty with environmental importance, and continues to inspire bird lovers and conservationists alike.
    </p>
</body>
</html>
temple.html
{% load static %}
<!DOCTYPE html>
<html>
<head>
    <title>Nattatreeswarar Temple</title>
    <style>
        body {
            background: linear-gradient(to right, #f1f8e9, #e8f5e9); /* soft gradient */
            font-family: "Georgia", serif;
            color: #2e7d32; /* deep green text */
            margin: 0;
            padding: 0;
        }
        h1 {
            text-align: center;
            color: #1b5e20; /* darker green for heading */
            padding: 25px;
            font-size: 2.8em;
            letter-spacing: 2px;
            text-shadow: 2px 2px #c8e6c9; /* subtle shadow for depth */
        }
        img {
            display: block;
            margin: 30px auto;
            width: 80%; /* responsive width */
            max-width: 850px;
            height: auto;
            border-radius: 20px;
            border: 5px solid #81c784; /* lighter green border */
            box-shadow: 0 6px 15px rgba(0,0,0,0.25); /* stronger shadow */
            transition: transform 0.3s ease-in-out;
        }
        img:hover {
            transform: scale(1.05); /* zoom effect on hover */
        }
        p {
            text-align: justify;
            line-height: 1.9;
            padding: 30px 60px;
            font-size: 18px;
            background-color: #ffffff;
            border-radius: 12px;
            margin: 30px auto;
            max-width: 950px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        }
    </style>
</head>
<body>
    <h1>Nattatreeswarar Temple</h1>
    <img src="{%static 'kovil.jpeg'%}" alt="Nattatreeswarar Temple">
    <p>
        Nattatreeswarar Temple is a revered Shiva temple located on a hillock island in the middle of the River Kaveri near Erode, Tamil Nadu.
        This ancient shrine, also called Nattātreeswarar or Natateshwarar Temple, is dedicated to Lord Shiva in the form of Agastheeswarar. 
        According to legend, Sage Agastya created a lingam out of sand on the hillock and worshipped it with his Rudraksha garland, seeking relief from doshas. 
        The temple is unique because it sits on a rocky island surrounded by the flowing waters of the Kaveri, accessible by a bridge, which makes the setting both spiritual and scenic.
        The temple is considered one of the Kongu Nadu’s Panchabhootha Sthalams, representing the element of earth (Prithvi). 
        Devotees believe that worshipping here removes obstacles and grants peace and prosperity. 
        The presiding deity, Lord Nattatreeswarar, is accompanied by Goddess Nallanayaki, and the temple is renowned for its Aadi Perukku festival, which celebrates the life-giving waters of the Kaveri.
        Architecturally, the temple follows the South Indian style, with a sanctum built in the Om shape on the hillock. 
        The natural surroundings, with the river encircling the temple, add to its charm, making it not only a place of worship but also a destination for those seeking tranquility and connection with nature.
        In essence, Nattatreeswarar Temple stands as a spiritual landmark of Erode, blending mythology, natural beauty, and cultural heritage, drawing devotees and visitors alike throughout the year.
    </p>
</body>
</html>
thindal.html
{% load static %}
<!DOCTYPE html>
<html>
<head>
    <title>Thindal Murugan Temple</title>
    <style>
        body {
            background-color: #f4f4f9; /* soft gray background */
            font-family: "Segoe UI", Arial, sans-serif;
            color: #333;
            margin: 0;
            padding: 0;
        }
        h1 {
            text-align: center;
            color: #4a148c; /* deep purple for a spiritual vibe */
            padding: 20px;
        }
        img {
            display: block;
            margin: 20px auto;
            width: 80%; /* responsive width */
            max-width: 700px;
            height: auto;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.2); /* subtle shadow */
        }
        p {
            text-align: justify;
            line-height: 1.8;
            padding: 20px 40px;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <h1>Thindal Murugan Temple</h1>
    <img src="{% static 'thindal.jpeg'%}" alt="Thindal Murugan Temple">
    <p>
        Thindal Murugan Temple, also known as Arulmigu Velayuthaswamy Thirukovil, is a famous hill temple in Erode dedicated to Lord Murugan.
Located on the scenic Thindalmalai hillock about 8 km from Erode town, the temple is one of the most revered shrines in the Kongu region of Tamil Nadu. The presiding deity here is Sri Velayudhaswami (Murugan), worshipped as the granter of prosperity and well-being. The temple stands at around 200 feet elevation and spreads across nearly 2.5 hectares, offering a panoramic view of the surrounding city. Historically, it began as a small shrine and gradually grew into a grand temple complex, now featuring a golden chariot (temple car) used during ceremonial processions.
The temple is not only a spiritual center but also a cultural landmark, attracting thousands of devotees year-round. It plays a vital role in Erode’s tourism, as many believe that a pilgrimage to Kongunadu is incomplete without visiting Thindal Murugan Temple. Festivals like Thaipusam and Panguni Uthiram are celebrated with great devotion, drawing crowds from across Tamil Nadu. With its Dravidian-style architecture, rich history, and divine atmosphere, Thindal Murugan Temple remains a symbol of faith and pride for the people of Erode.
Would you like me to expand this into a short essay-style description highlighting its history, architecture, and festivals in more detail? That way, you’ll have a fuller picture of why Thindal is so special.

    </p>
</body>
</html>
# OUTPUT

![map html](https://github.com/user-attachments/assets/c818d747-1716-48b7-aebd-d506c852a687)

![park html](https://github.com/user-attachments/assets/e1b42cda-bfb4-456c-9060-b75e4c0d0d6e)

![sant html](https://github.com/user-attachments/assets/b5f91a28-55df-4ffb-a80a-ca9648e7f72a)

![temple html](https://github.com/user-attachments/assets/c7d3ece7-9db6-4b9f-9071-54e5de961984)

![thindal html](https://github.com/user-attachments/assets/eed8c88d-4814-488b-8557-18cf13d7b601)

# RESULT
The program for implementing image maps using HTML is executed successfully.
