# EXP 02 - CREATING A COMMERCIAL WEBSITE USING HTML & CSS
## AIM:

To create a commercial website using html and css.

## SOFTWARE:

Visual Studio Code.

## ALGORITHM:

### 1) Create a new HTML file and save it with a .html extension.Begin with the basic structure by adding the <!DOCTYPE html> declaration at the top.
### 2) Set up the Head:

### Inside the head element, add the title element and give it a meaningful title for your website. Link your CSS file by adding the <link> element with the rel attribute set to "stylesheet" and  the href attribute pointing to your CSS file.

### 3) Develop the Content:
###  Divide the main content area into sections using appropriate HTML elements like section, div, or article. Use headings h1 to h6 to structure your content hierarchically. Incorporate text, images, videos, and other media within the content sectionS


### 4) Style with CSS:
 
###  Create a new CSS file and save it with a .css extension.
###  Select the elements you want to style using CSS selectors.
###  Apply styles using properties and values. 
###  For example, you can change colors, fonts, sizes, margins, and padding.

### 5) Find a web hosting provider to host your website online.
### Upload your HTML, CSS, and any other necessary files to the hosting server.

### 6) Test your website again after deployment to ensure it works as intended.
## PROGRAM:
### HTML:
```
<!DOCTYPE html>
<html>
    <head>
        <title>Starry night</title>
        <link rel="icon" href="./moon.jpg" type="icon" />
        <link href="./styling.css" rel="stylesheet">
    </head>
    <body style="background-color: rgb(7, 7, 7)">
        <div style="background-image: url(./background2.jpg); background-size: cover; border-radius: 25px; padding-bottom: 160px;">
            <div class="header">
                <div class="menu">
                    <img src="./icons8-signal-100.png" style="height: 35px; width: fit-content">
                </div>
                <div class="menu">
                    Offers
                </div>
                <div class="menu">
                    Explore
                </div>
                <div class="menu">
                    Contact us
                </div>
                <div style="padding-left: 850px;">
                    <div class="menu" style="border: 1px solid white; border-radius: 65px;">
                        Login
                    </div>
                </div>
            </div>
            <div style="padding-top: 90px;">
                <div class="bts1">
                    Explore the life you want<br> to live<br>Put your money to work.<br><br>
                    <div style="padding-left: 150px;">   
                        <div class="photoanimate"></div>
                    </div> 
                </div>
            </div>
            <div style="padding-left: 170px; padding-top: 50px;">
                <div class="enroll">
                    ENROLL
                </div>
            </div>
        </div>
    <!---Offers -->
        <p style="font-size: 50px; color: rgb(251, 251, 251); padding-left: 50px;font-family: 'Bruno Ace', cursive;
        font-family: 'Sigmar', cursive;">Black Advantage</p>
        <div class="offer">
            <div class="offer_box">
                <div class="offer_text">
                    <img src="./medal.png" type="icon">
                    <p style="font-size: 25px;">Financial Experience</p>
                    <p style="font-size: medium;color: rgb(182, 209, 253);">Expertise in finance can contribute to a company's short-term success by facilitating cash flow and to its long-term success by lessening interest payments and finance charges. </p>
                </div>
            </div>
            <div class="offer_box">
                <div class="offer_text">
                    <img src="./tech.png" type="icon">
                    <p style="font-size: 25px; ">Advanced technology</p>
                    <p style="font-size: medium; color: rgb(199, 218, 250);"> Integrated learning systems accelerate the learning process of the students. Technology for schools incorporates the use of unique approach in-class activities using multimedia content and this develops a learning eagerness among the students.</p>
                </div>
            </div>
            <div class="offer_box">
                <div class="offer_text">
                     <img src="./ai.png" type="icon">
                     <p style="font-size: 25px;">Right Advice</p><p style="font-size: medium; color: rgb(199, 218, 250);">Seeking and giving advice are central to effective leadership and decision making. Yet managers seldom view them as practical skills they can learn and improve. </p>
                 </div>
             </div>
        </div>
        <br><br><br>
    
    <!---Explore-->
    <div style="background-image: url(./background.jpg); padding-bottom: 150px; border-radius: 25px; opacity: 0.; background-size: cover;">
        <div class="header">
            <div style="font-size: 25px; width: 500px; padding-top: 100px; padding-left: 130px;">
                <div class="menu" style=" width:fit-content">ANALYSIS OF YOUR WEALTH</div>
            </div>
        </div>
        <div class="thirdpage" style="font-size: 50px;">
            Helping you to connect the dots,<br>
            So, yoou can see what life <br>
            could look like into the future.
            <br>   <br><br>
            <div style="font-size: 20px; width: 800px; color: rgb(183, 228, 248);">
                Self-evaluation is the process of systematically observing, analyzing and improving one’s own actions or results. Self-evaluation takes place at an individual level, but also at a department or organizational level.
    In the workplace, this method concretely means examining and evaluating one’s own professional contributions. Various definitions are given to self-evaluation, but all include the features described above.
            </div>
        </div>
    </div>
    </body>
</html>
```
### CSS stylesheet:
```

.header {
    display: flex;
    padding: 20px;
    justify-content: flex-start;
    align-items: flex-start;
    text-align: center;
    opacity: 100%;
    border-radius: 10px;
  }
.menu{
    display: flex;
    justify-content: space-around;
    align-items:flex-start;
    width: 120px;
    border-radius: 10px;
    font-family: 'DynaPuff', cursive;
    padding: 10px;
    font-size: 22px;
    font-weight: bold;
    color: rgb(254, 253, 254);
}
a{
    text-decoration: none;
    color: white;
}
.menu:hover{
    background-color: rgb(255, 253, 253);
    color: black;
    animation: buttonup1 infinite;
    animation-duration: 0.6s;
    animation-direction:alternate;
    
}
@keyframes buttonup1 {
    from {top: 0px;}
    to {top: 10px;}
  }  
.bts1{
    display: inline-flex;
    padding-top: 100px;
    padding-left: 160px;
    align-items: center;
    font-size: 70px;
    color: rgb(255, 255, 255);
}
.photoanimate{
    align-content:normal;
    animation: photocg 10s infinite;
    animation-direction: normal;
    width: 200px;
    height: 150px;
    border-radius: 45px;
    box-shadow: 5px 6px 5px rgb(204, 225, 244);
}
@keyframes photocg{
    0%{
        background-image: url(./galaxy.jpg);
        transform: translate(0%,0%);
        background-size: cover;
    }
    5%{
        background-image: url(./background.jpg);
        transform: translate(120%,150%);
        background-size: cover;
    }
    15%{
        background-image: url(./galaxy.png);
        transform: translate(0%,140%);
        background-size: cover;
    }
    23%{
        background-image: url(./galaxy2.jpg);
        transform: translate(120%,120%);
        background-size: cover;
    }
    36%{
        background-image: url(./galaxy3.jpg);
        transform: translate(0%,0%);
        background-size: cover;
    }
    48%{
        background-image: url(./galaxy4.jpg);
        transform: translate(120%,-120%);
        background-size: cover;
    }
    56%{
        background-image: url(./galaxy5.jpg);
        transform: translate(0%,-140%);
        background-size: cover;
    }
    66%{
        background-image: url(./galaxy6.jpg);
        transform: translate(120%,-160%);
        background-size: cover;
    }
    77%{
        background-image: url(./galaxy7.jpg);
        transform: translate(0%,-180%);
        background-size: cover;
    }
    88%{
        background-image: url(./bg2.jpg);
        transform: translate(120%,-160%);
        background-size: cover;
    }
    99%{
        background-image: url(./bg3.jpg);
        transform: translate(0%,-140%);
        background-size: cover;
    }
    100%{
        background-image: url(./galaxy4.jpg);
        transform: translate(0%,0%);
        background-size: cover;
    }

}
.enroll{
    display: flex;
    justify-content: space-around;
    border: 1px dotted white;
    border-radius: 25px;
    font-size: 19px;
    font-weight: bold;
    color: rgb(250, 250, 250);
    text-align: center;
    padding: 15px;
    width: 100px;
    background-color: rgb(7, 7, 7);
    
}
.enroll:hover{
    background-color: aliceblue;
    color: rgb(7, 7, 7);
}
.offer{
    display: flex;
    justify-content: space-evenly;
    padding-bottom: 20px;
    
}
.offer_box{
    display: flex;
    padding: 5px;
    width: 300px;
    
}
.offer_text{
    color: rgb(253, 252, 253);
    font-size: 30px;
    font-family: 'Bruno Ace', cursive;
    padding: 10px;
    background-size: 1920px 1020px;
}
.thirdpage{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    padding-top: 100px;
    padding-left: 150px;
    font-size: 70px;
    color: rgb(255, 255, 255);
}
```
## OUTPUT:
![Web capture_9-6-2023_85857_127 0 0 1](https://github.com/gpavithra673/Exp_02_Creating_commercial_website/assets/93427264/82170f10-59b3-4ec3-82ec-33eece3be8a1)

## RESULT:
      
Thus the website is created.



 
