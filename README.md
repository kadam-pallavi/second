# second

# My-project
This is my project
# Personal-Portfolio-Website

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Personal Portfolio Website</title>
    <!----CSS link----->
    <link rel="stylesheet" href="style.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}
a{
    text-decoration: none;
}
.hero{
    width: 100%;
    height: 100vh;
    background: url(img/bg1.jpg);
    background-size: cover;
}
nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 30px 100px;
}
.logo{
    max-height: 60px;
}
nav ul li{
    list-style: none;
    display: inline-block;
    padding: 10px 20px;
}
nav ul li a{
    color: #1d1d24;
    position: relative;
    padding: 5px 0;
}
nav ul li a:hover{
    color: #fd4766;
}
nav ul li a:after{
    content: "";
    position: absolute;
    left: 0;
    width: 0;
    height: 3px;
    background: #fd4766;
    transition: .3s;
    bottom: 0;
}
nav ul li a:hover:after{
    width: 100%;
}
.btn{
    color: #fff;
    font-size: 16px;
    text-transform: uppercase;
    letter-spacing: 2px;
    padding: 16px 40px;
    border-radius: 500px;
    display: inline-block;
    font-weight: 500;
    transition: all .4s ease-in-out;
    background-size: 152% 100%;
    background: #fd4766;
    border: 2px solid #fd4766;
}
.btn:hover{
    background: transparent;
    border-color: #fd4766;
    color: #fd4766;
}
.content{
    position: absolute;
    top: 35%;
    left: 8%;
}
.content .title{
    color: #1f1f25;
    font-size: 15px;
    text-transform: uppercase;
    letter-spacing: 4px;
    display: inline-block;
    margin-bottom: 20px;
    background: linear-gradient(120deg, #1c99fe 20.69%, #7644ff 50.19%,#fd4766 79.69%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}
.content h1{
    color: #1f1f25;
    font-size: 75px;
    font-weight: 900;
    line-height: 90px;
    text-transform: inherit;
    width: 70%;
}
.content h1 span{
    color: #fd4766;
}
.content p{
    width: 55%;
    color: #757575;
    margin-top: 25px;
    margin-bottom: 30px;
}

    </style>
</head>
<body>

    <div class="hero">
        <nav>
            <img src="https://tse2.mm.bing.net/th?id=OIP.XLEV-RfC1UqSF4bWuhD34wHaHa&pid=Api&P=0"
             class="logo">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Service</a></li>
                <li><a href="#">Portfolio</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
            <a href="#" class="btn">Buy Now</a>
        </nav>

        <div class="content">
            <span class="title"> Web Developer</span>
            <h1>Hello, I’m <span>Pallavi</span></h1>
            <p>I’m working on a perspnal portfolio website, visually sophisticated and technologically proficient, responsive and multi-functional React Template Imroz.</p>
            <a href="#" class="btn">Download CV</a>
        </div>
    </div>

</body>
</html>


# Mobile Navigation Frontend

<!--html part-->
<!DOCTYPE html>
<html lang="en">
<head></head>
<body>
    <div class="phone">
        <img src="https://images.unsplash.com/photo-1480074568708-e7b720bb3f09?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1053&q=80" 
        alt="home" class="content show">
        <img src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80"
         alt="work" class="content">
        <img src="https://images.unsplash.com/photo-1471107340929-a87cd0f5b5f3?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1266&q=80"
         alt="blog" class="content">
        <img src="https://yt3.ggpht.com/ytc/AKedOLQcC81-nEY5of9YYjoL3l8uKO_QUhag_Yy0KYvz=s900-c-k-c0x00ffffff-no-rj"
         alt="about" class="content">
        <nav>
            <ul>
                <li class="active">
                    <p>Home</p>
                </li>
                <li>
                    <p>Work</p>
                </li>
                <li>
                    <p>Blog</p>
                </li>
                <li>About Us</li>
            </ul>
        </nav>
    </div>
</body>
</html>

<!--CSS PART--->
*{
    box-sizing: border-box;
}
body {
    background-color: #222457;
    font-family: 'Open Sans', sans-serif;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    margin: 0;
}
.phone {
    position: relative;
    overflow: hidden;
    border: 3px solid #eee;
    border-radius: 15px;
    height: 600px;
    width: 340px;
}
.phone .content{
    opacity: 0;
    object-fit: cover;
    position: absolute;
    top: 0;
    left: 0;
    height: calc(100% -60px);
    width: 100%;
    transition: opacity 0.4s ease;

}
.phone .content.show {
    opacity: 1;

}

nav {
    position: absolute;
    bottom: 0;
    left: 0;
    margin-top: -5px;
    width: 100%;
}

nav ul  {
    background-color: #fff;
    display: flex;
    list-style-type: none;
    padding: 0;
    margin: 0;
    height: 60px;
}

nav li {
    color: #6461a2;
    cursor: pointer;
    flex: 1;
    padding: 10px;
    text-align: center;
}

nav ul li p {
    font-size: 12px;
    margin: 2px 0;

}

nav ul li:hover, nav ul li:active {
    color: #8e44ad;
}

});

<!-- js -->
const contents = document.querySelectorAll(".content");
const listItems = document.querySelectorAll("nav ul li");
const hideAllContents = () => {
  contents.forEach((content) => content.classList.remove("show"));
};
const hideAllItems = () => {
    listItems.forEach((item) => item.classList.remove("active"));
};
listItems.forEach((item, index) => {
  item.addEventListener("click",() => {
      hideAllContents();
      hideAllItems();
      item.classList.add("active");
      contents[index].classList.add("show");
  });
});
