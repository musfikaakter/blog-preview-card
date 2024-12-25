I tried to set that black shadow behind the box using ::after/ ::before pseudo class(I actually tried using both), but it didn't work out. I did a project like this before and it worked on that very well, in every browser. I'm using Chrome, Firefox, Opera and Edge. I'm using the latest versions of all. But this time it didn't work att all. If anyone has any solution then kindly help me out!

.box {
    position: relative;
    height: 31.25rem;
    width: 20.4375rem;
    border: 1px solid var(--blackish);
    border-radius: 1.25rem;
    background-color: rgb(255, 255, 255);
}

.box::after {
    content: '';
    position: absolute !important;
    top: 0.4rem;
    left: 0.4rem;
    height: 31.25rem;
    width: 20.4375rem;
    border-radius: 1.25rem;
    background-color: rgb(0, 0, 0);
    z-index: -1;
}