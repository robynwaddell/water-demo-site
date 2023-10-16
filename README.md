# Demonstration of HTML and CSS   
## What Our Website Is For   
It is a website for a water company that specializes in water for people with active and busy lifestyles. It focuses on healthy, pure and sustainable hydration for any and all situations. It features three lines of products and a water subscription option. Our page features an index and home page, a contact page and an about us page.  
## The Audience  
The creation of this site is to display our HTML and CSS coding ability and creativity with design only elements. It was made to fit the rubric of our assignment but in terms of the target audience it is designed for athletes, extreme hobbyists, and anyone who leads a life where hydration is achieved with optimal efficiency and quality.  
## The Goal  
When creating this assignment we wanted to make sure it looked as professional and polished as possible. To do so we sat down on the first day and decided our stylistic choices  and mapped out the website so that everyone was on the same page. It was important to us that every decision and piece of code had purpose and was somehow related back to our main goal of creating an industry level page.  
## Our Challenges  
The most difficult aspect to our page was the CSS waves on the hero banner, they were something that as a partnership, we both researched many options before settling on one, and then implementing it. Another struggle  for me personally was the `flex` function in CSS it took me quite a while to get the proportions right and make sure everything was well aligned. I think as a partnership we struggled a lot with communication and with using GitHub to simultaneously work on projects. I had never previously used it before so it was a learning curve for me and my partner wasn’t used to teaching or explaining these beginner steps so I believe she found it a touch frustrating. However, we got there in the end and I am quite proud of our accomplishments.  
### Here is an exerpt of code from our index page on how we wrote the HTML for the waves affect   
```
<div class="waves-container">
                <svg class="waves" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
                viewBox="0 24 150 28" preserveAspectRatio="none" shape-rendering="auto">
                <defs>
                    <path id="gentle-wave" d="M-160 44c30 0 58-18 88-18s 58 18 88 18 58-18 88-18 58 18 88 18 v44h-352z" />
                </defs>
                    <g class="parallax">
                        <use xlink:href="#gentle-wave" x="48" y="0"/>
                        <use xlink:href="#gentle-wave" x="48" y="3"/>
                        <use xlink:href="#gentle-wave" x="48" y="5"/>
                        <use xlink:href="#gentle-wave" x="48" y="7"/>
                    </g>
                </svg>
            </div>
```  
The code here is what makes the waves on the home page. It gives them ther shapes and sets up the framework for CSS
to come in and use things like 
* `transition`
* `background-color`
* `animation`  
## The Future Improvements  
Some improvements I would want to make moving forward, would be to clean up the alignment and create more separation between sections, recolour the links, add more little details such as validation to the form, and other aesthetic details. I also would want to spend more time on the assets, such as pictures and videos. I feel that our page would be much more elevated if it had more images and I think that a video in the home page and then moving the CSS waves to the contact and about-us pages would be better. I also want to have more modern looking sections in terms of better use of subtler shadows and color because I think it still looks just a touch juvenile at the moment. I think I would also want to take a look at this particular section of code and refine it some more.  
### This is an exerpt from our index page HTML  
```
<section class="section-three">
            <div>
                <h2>Our Product Lines</h2>
            </div>
            <div class=" box collection-one">
                <img src="./assets/img/flavourburst.png">
                <div>
                 <h2>Flavourburst</h2>
                 <p> Flavourburst is our line of fruit and her infused waters. Featuring Grapefruit-mint, 
                    Blackberry-sage, and Peach-tea.
                </p>
                </div>
                <input type="button" class="primary-button" value="View Collection">
            </div>
            <hr>
            <div class=" box collection-two">
                <img src="./assets/img/elevate.png">
                <div>
                 <h2>Elevate</h2>
                 <p> Energizing, refreshing and enhancing, Elevate was made for anyone searching for peak 
                    performance. 
                </p>
                </div>
                <input type="button" class="primary-button" value="View Collection">
            </div>
            <hr>
            <div class=" box collection-three">
                <img src="./assets/img/vita.png">
                <div>
                 <h2>Vita</h2>
                 <p> Vita is a carefully crafted, ph balanced, mineral infused line of waters for healing the body 
                    with hydration.
                </p>
                </div>
                 <input type="button" class="primary-button" value="View Collection">
                </div>
                <hr>
        </section>
```  
This section is what made the product line section. Each `div` is essentially one of the products. They are all labelled with a class name. A `class` is a naming tool that we use to specify a particular section of code. Any CSS
principles applied to the class, appearing as this in the code `.classname` will affect anything within the element 
that has the class. This concept is often refered to as parent and child elements. `div class = 'box collection-three` is the parent and everything it contains is the child. In this instance our `div` is labelled with `class = 'box collection-three`. This gives it two classes. `box` and `collection-three`. Thus any CSS we apply to `box` will also apply to the images, paragraphs, headings and buttons within it. Usually this is used to apply things like:
* `flex` 
* `margin`
* `height`
* `width`  

As well as being used to help with reactivity when it comes to viewport size.  


Within the CSS I would specifically like to improve my understanding of our document and refine it a bit more, likely with more variables. I think that because having two people working on it at the same time, I may have gotten a bit confusing or unreadable at times. For example this is a section I would like to change.  
### This is from our style CSS page
```
.section-one, .section-two {
    display: flex;
    gap: 20px;
    justify-content: center;
    align-items: center;
    padding: 30px;
    border-radius: 10px;
}
.section-three {
    display: flex;
    flex-direction: column;
    gap: 20px;
    justify-content: center;
    align-items: center;
    padding: 30px;
    border-radius: 10px;
    width: 90%;
    margin-top: 60px;
}

.section-img {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20px;
    flex-wrap: wrap;
}

.section-one.brand-message {
    width: 50%;
}

.section-one {
    padding: 40px 40px;
    border-radius: 6px;
}

.section-one h2 {
    color: var(--primary-orange);
}

.section-img, .section-two {
    margin-top: 120px;
}

.section-two h2 {
    color: #fff;
    font-size: 36px;
}

.section-one.three-quarters {
    width: 80%;
    margin-inline: auto;
    margin-top: 60px;
}

.founders.three-quarters {
    width: 75%;
    margin-inline: auto;
    margin-top: 60px;
}

hr {
    margin: 0 auto;
    width: 100%;
    border: 0;
    height: 1px;
    background-image: linear-gradient(to right, rgba(255, 255, 255, 0), var(--secondary-blue) , rgba(255, 255, 255, 0));
}

.section-two.row {
    padding: 20px 0px;
}

.row {
    display: flex;
    flex-wrap: wrap;
  }

.column {
    flex: calc(25% - 15px);
}
  
.column {
    -webkit-box-align: center;
    align-items: center;
    background: rgb(255, 255, 255);
    border-radius: 16px;
    box-shadow: rgba(0, 0, 0, 0.1) 0px 8px 24px 0px;
    display: flex;
    flex-direction: column;
    overflow: hidden;
    padding-bottom: 20px;
    position: relative;
}

.column-title {
    color: rgb(56, 56, 56);
    padding: 12px 0px;
    text-align: center;
    font-weight: 900;
    font-size: 18px;
    background: linear-gradient(60deg, rgb(62 92 230) 9%, rgb(110 167 255) 100%);
    width: 100%;
}

.column img {
    margin-top: 25px;
    width: 70%;
    padding: 20px;
    border-radius: 10px;
    background-color: #5c9cfd1a;
}

.column p {
    text-align: center;
    padding: 10px;
    height: 75px;
}

.index-img {
    width: 400px;
    height: 300px;
    border-radius: 10px;
}

.column h3 {
    font-family: 'Xeroda', sans-serif;
    font-size: 50px;
}

.box {
    -webkit-box-align: center;
    width: 100%;
    height: 200px;
    align-items: center;
    display: flex;
    overflow: hidden;
    padding: 20px;
    position: relative;
    gap: 15px;
}

.box img {
    height: 200px;
    width: 300px;
    margin-right: 15px;
}

.box div {
    width: 50%
}

```

I would condense some of the sections and break is down into sections, columns and boxes, divided with comments.
I would also make the names more specific and helpful to people who are just viewing our code for the first time.

