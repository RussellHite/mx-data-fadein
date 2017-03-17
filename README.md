# mx-data-fadein
Sass function/mixin that allows you to sequentially animate in listview items
View icons: https://material.io/icons/

## Prerequisites
For easiest implementation of this or any other icon font it is reccomended you install the Vanilla theme when you start to style your applicaton.
https://appstore.home.mendix.com/link/app/2681/Mendix/Vanilla-Theme

## Configuration
Here are the steps to incorporate this partial into your project. 

### Step 1
Copy and paste the _fade-in.scss file into the following folder your_project_folder/theme/styles/sass/lib/components
### Step 2
Open the lib.scss file under your_project_folder/theme/styles/sass and under the bottom add the following line:
```
@import "components/fade-in";
```
to include the _fade-in.scss file partial into the outputed css file
### Step 3
To use this sass mixin add this line within a listview starting brackets
```
.mx-listview {
    @include fade-in($number: 50, $anime-time: .5s, $delay-time: .3s);
}
```
Change $number value to match the page size of the listview,
       $anime-time value to be the time it takes for an item to fade in,
       $delay-time value to be the time between each items fade in.