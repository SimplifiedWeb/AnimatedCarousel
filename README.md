# AnimatedCarousel

so basaically this is a simple animated carousel.

> step1 => In the project you see that when we change
the picture the background picture is also get changed.
> So if you Know that how the carousel work then
it is easy to understand how we set the background Image
just changin the body.background. 

> So we have to two things in the slider one is the
right and the other one is the left.

Now always remember that when we have tons of things that we wanna 
show one by one in order sequence so we always gonna use the Array.

<div class="slide active" style="background-image: url('container-1.jpg')">
</div>

simple we have 5 divs like this only one at a time has a active class.

So in Javascript,

Always remember we have to maintain a state.
we get all the elements through querySelectorAll that give us nodeList, which
is any array like object not an original array, but we can use forEach methods
in modern browsers.

Steps-1: -> One function used to change the body of the background.
steps-2: -> One Function used to change The state when we click on the left or right.
steps-3: -> One function used to go to Next image
steps-4: -> One function used to go back to previous image.
leftButton.addEventListener("click",()=>{
    activeSlide--;
    if(activeSlide < 0) activeSlide = slides.length - 1;
    setBackground()
    setActiveSlide()
})

so if our activeSlide is 0 and you clicked left to see the last image, we simple
said if the activeSlide is 0 and click on the left one we decrement that activeSlide state,
which is going 0 to -1 and then we check the condition activeSlide < 0 condition was true right
bcz activeSlide is now -1 and zero is greated than -1 that how it show the last image.

and we set all the div images to opacity 0 only the active class has the 
opacity 1.

Hope this explanation understand.





