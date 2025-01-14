 <h1 align="center">shinsouhitoshi1203　／　basic swiper </h1>
 
## 0. what is swiper
swiper is a useful **library** for making slideshow in website without wasting time building your slideshow modules.
take this one as an example:

<img  src="https://user-images.githubusercontent.com/12080141/180462341-0ca850ae-a761-4587-bb93-8379e053be25.gif">

## 1. getting started

### a. install swiper

#### for static websites
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css">
<script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
```

### b. configure a swiper

#### ・basic structures

![image](https://github.com/user-attachments/assets/74752470-7ffa-4919-b489-5f7b9bc77f81)

#### ・javascript configuration
basic structures
```js
const swiper02 = new Swiper (
    [selector parent having the .swiper class],
    {
		// parameters here are grouped as an object
        direction: "horizontal",  // direction
        grabCursor: true,          //  cursor: grab
        autoplay: {  
            delay: 3000               //  wait 3s until it navigates to the next slide 
        },
        speed: 1000,                //  1s to switch to the next slide
        // [...]
    }
 )
```

## 2. parameters for configuring objects
> [!NOTE]
> for the inputs of the parameter, remember to keep the inputs as much natural as they are. for instances, if you want to input **horizontal**, or **true**, or **123**, just type `'horizontal'`, `true` and `123`, respectively.

|  parameter  |  input requirement  |  usages  |  examples |
| :------------: | :------------: | ------------ | :------------: |
|  `direction` |  `'horizontal'` or `'vertical'` | indicate the direction of navigation  |   |
|  `grabCursor` |  `boolean` |  allow to use the grab cursor during swiping, *highly recommended for UX* |   |
|  `speed` |  `number (miliseconds)` |  determine the amount of time enough<br> to completely navigate to the next slide  |  |
|  `watchOverflow` | `boolean`  |  decide if you want to keep sliding despite having only one slide | [click here](https://stackblitz.com/edit/stackblitz-starters-zdjfxz "click here") |
|   |   |   | |
