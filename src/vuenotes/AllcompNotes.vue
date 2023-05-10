<template>
  <div>

<h3>COMPONENT- ALERT</h3>
<div>
    <v-alert
    border="top"
  color="orange"
  icon="mdi-plus"                 
  text
  outlined
  prominent
  shaped
  elevation="24"
    > 
    I'm an Alert Usage Example
</v-alert>
<p>
  border="top"       // Only border will change <br/>
  color="orange"       // For adding color <br/>
  dense                // Alert become thin <br/>
  prominent           //  Alert become fat <br/>
  icon="mdi-plus"     // For Adding Icon        <br/>    
  text                // Just change color  <br/>
  outlined            // Just Outline to alert  <br/>
  shaped              // Alert shape will be change <br/>
  elevation="24"      // Back Shadow on alert
</p>      
</div>

<br/>
<hr/>
<br/>

<h3>COMPONENT- v-app</h3>
<p>In order for your application to work properly, you must wrap it in a v-app component. This component is required for ensuring proper cross-browser compatibility. There should only be one and it must be the parent of ALL Vuetify components.
<br />
    Below is a list of all the components that support the app prop and can be used as layout elements in your application.
<br />
1. v-app-bar <br/>
: Is always placed at the top of an application with a lower priority than v-system-bar. <br />
2. v-bottom-navigation <br/>
: Is always placed at the bottom of an application with a higher priority than v-footer. <br />
3. v-footer <br/>
: Is always placed at the bottom of an application with a lower priority than v-bottom-navigation. <br />
4. v-navigation-drawer <br/>
: Can be placed on the left or right side of an application and can be configured to sit next to or below v-app-bar. <br />
5. v-system-bar <br/>
: Is always placed at the top of an application with higher priority than v-app-bar.   <br/>     
</p>

<br/>
<hr/>
<br/>

<v-avatar
  color="primary"
  size="56"
  tile
></v-avatar>

<h3>COMPONENT- Avatars</h3>
<p> 
color="primary"   // Add Color <br/>
size="56"        // Increase Size <br/>
tile             // Make in a tile format or square shape  <br/>
rounded          // Make in a round shape  <br/>

The v-avatar component is typically used to display circular user profile pictures. This component will allow you to dynamically size and add a border radius of responsive images, icons, and text. A tile variation is available for displaying an avatar without border radius.</p>

<br/>
<hr/>
<br/>


<h3>COMPONENT- v-app-bar</h3>
<div>
    <v-app-bar
      color="deep-purple accent-4"
      dense
      dark
    >

    <!-- This is used to add the NAV Icon  (3 lines icon) -->
      <v-app-bar-nav-icon></v-app-bar-nav-icon>     
    
    <!-- For adding the title    -->
      <v-toolbar-title>Page title</v-toolbar-title>

    <!-- For adding the space   -->
      <v-spacer></v-spacer>


    <!-- for small icons   -->
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>


      <v-menu
        left
        bottom
      >
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            icon
            v-bind="attrs"
            v-on="on"
          >
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item
            v-for="n in 5"
            :key="n"
            @click="() => {}"
          >
            <v-list-item-title>Option {{ n }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
</div>

<p>The v-app-bar component is pivotal to any graphical user interface (GUI), as it generally is the primary source of site navigation
<br/>
<b>API</b>    <br/>
1. v-app-bar  <br/>
2. v-app-bar-nav-icon  <br/>
3. v-app-bar-title  <br/>


<b>PROPS</b>  <br/>
Collapsible bars <br/>
Dense  <br/>
Elevate on scroll  <br/>
Fade image on scroll  <br/>
Hiding on scroll  <br/>
Images  <br/>
Inverted scrolling  <br/>
Prominent  <br/>
Scroll threshold  <br/> 
</p>


<br/>
<hr/>
<br/>

<h3>EXTRA</h3>
<p>
    class="mx-auto"   // Adding margin from right and left  <br/>
    width="200px"     // Can give width to any tag   <br/>
    height="100"      // Can give height to any tag   <br/>
    max-width="200"   // Can give max-width to any tag  <br/>
    class="pa-md-4 mx-lg-auto"      <br/>
</p>

<br/>
<hr/>
<br/>

<h3>SPACING IN PADDING AND MARGIN</h3>

<p>
  0 - eliminates all margin or padding by setting it to 0 <br/>
  auto - sets the spacing to auto <br/>
  1. size 1- 4px in Vuetify  <br/>

pr-7   -> padding on right side <br/>
ps-7  -> padding on left side   <br/>
px-7  -> left and right   <br/>
py-7  -> top and bottom  <br/>
pa   -> all side  <br/>
</p>

<br/>
<hr/>
<br/>

<h3> BREAKPOINTS </h3>
<p>
    
1. Extra small -> xs -> Small to large -> phone -> (less than 600px).  <br/>
2. Small  ->  sm -> Small to medium -> tablet -> (Inbetween 600px to 960px)  <br/>
3. Medium -> md	-> Large tablet to laptop -> (960px to 1264px)*   <br/>
4. Large -> lg -> Desktop -> (Inbetween 1264px to 1904px)  <br/>
5. Extra large -> xl -> 4k and ultra-wide ->  (Above 1904px)  <br/>
</p>


<br/>
<hr />
<br/>

<h3> VISIBILITY </h3>
<p>
Conditionally display an element based upon the current viewport. Breakpoint utility classes always apply from the bottom up. That means if you have .d-none, it will apply to all breakpoints. However, .d-md-none will apply to only md and up.
<br/>

1. Hidden on all  -> 	.d-none   <br/>
2. Hidden only on xs  -> 	.d-none .d-sm-flex   <br/>
3. Hidden only on sm ->	.d-sm-none .d-md-flex  <br/>
4. Hidden only on md ->	.d-md-none .d-lg-flex  <br/>
5. Hidden only on lg ->	.d-lg-none .d-xl-flex  <br/>
6. Hidden only on xl ->	.d-xl-none   <br/>
7. Visible on all ->	.d-flex  <br/>
8. Visible only on xs ->	.d-flex .d-sm-none   <br/>
9. Visible only on sm ->	.d-none .d-sm-flex .d-md-none   <br/>
10. Visible only on md ->	.d-none .d-md-flex .d-lg-none  <br/>
11. Visible only on lg ->	.d-none .d-lg-flex .d-xl-none1 <br/>
12. Visible only on xl ->	.d-none .d-xl-flex  <br/>
</p>

<br/>
<hr/>
<br/>

<h3>TEXT & TYPOGRAPHY</h3>
<p>
  class="font-weight-medium"      // Font weight <br/>
    class="text-h1"           // adding h1  <br/>
    
    <br/>
    
    These classes can be applied to all breakpoints from xs to xl. When using a base class, .text-{value}, it is inferred to be .text-xs-${value}.
    <br/>
.text-{value} for xs <br/>
.text-{breakpoint}-{value} for sm, md, lg and xl <br/>

<br/>

The value property is one of:
<br/>
    h1 <br/>
    h2 <br/>
    h3 <br/>
    h4 <br/>
    h5 <br/>
    h6 <br/>
    subtitle-1 <br/>
    subtitle-2  <br/>
    body-1  <br/>
    body-2  <br/>
    button  <br/>
    caption  <br/>
    overline  <br/>

</p>

<br/>
<hr/>
<br/>

<h3>TEXT ALINGMENT</h3>
<p>
  Alignment helper classes allow you to easily re-align text. <br/>
    class="text-left"  // This is how we use  <br/>
    <br/>
    PROPERTIES- <br/>
    text-left <br/>
    text-center <br/>
    text-right  <br/>

    <br/>

    <b>FOR RESPONSIVE</b>  <br/>
    text-sm-left   <br/>
    
    <br/>

    <b>TRANSFORMATION</b>  <br/>
    <br/>
    class="text-lowercase"   // This is how we use   <br/>
    text-uppercase   <br/>
    text-capitalize   <br/>

</p>

<br/>
<hr/>
<br/>

<h3>OVERFLOW</h3>
<p>
  Specify the elements overflow, overflow-x, or overflow-y property.   
<br/>
Where overflow refers to the type: overflow, overflow-x or overflow-y and value can be one of: auto, hidden, or visible
<br/>
    class="overflow-auto"    // This is how we use   <br/>
    overflow-auto              // is used to add scrollbars to an element when its content overflows the bounds  <br/>
    overflow-hidden            // content will not scroll  <br/>
    overflow-visible           // content will seen out of the box or card  <br/>
    overflow-x-auto   <br/>
    overflow-x-hidden  <br/>
    overflow-x-visible  <br/>
    overflow-y-auto  <br/>
    overflow-y-hidden  <br/>
    overflow-y-visible   <br/>
    class="purple darken-2 "   // Giving Background Color   <br/>
    class="text-center"  //For Text-center   <br/>
    class="white--text"   // For changing text color   <br/>
</p>

<br/>
<hr/>
<br/>

<h3>FLEX PROPERTIES</h3>
<p>
  Column, row & reverse  
  <br/>
  class="d-flex flex-row"   //For Flex Row   
  <br/>
    class="d-flex flex-column"  // For adding columns   
<br/>
    There are also responsive variations for flex-direction.   
<br/>
    .flex-row   <br/>
    .flex-row-reverse   <br/>
    .flex-column   <br/>
    .flex-column-reverse   <br/>
    .flex-sm-row   <br/>
    .flex-sm-row-reverse   <br/>
    .flex-sm-column   <br/>
    .flex-sm-column-reverse   <br/>
    .flex-md-row   <br/>
    .flex-md-row-reverse   <br/>
    .flex-md-column   <br/>
    .flex-md-column-reverse   <br/>
    .flex-lg-row   <br/>
    .flex-lg-row-reverse   <br/>
    .flex-lg-column   <br/>
    .flex-lg-column-reverse   <br/>
    .flex-xl-row   <br/>
    .flex-xl-row-reverse   <br/>
    .flex-xl-column   <br/>
    .flex-xl-column-reverse   <br/>

</p>

<br/>
<hr/>
<br/>

<h3>FLEX JUSTIFY</h3>
<p>
  The justify-content flex setting can be changed using the flex justify classes. This by default will modify the flexbox items on the x-axis but is reversed when using flex-direction: column, modifying the y-axis.
<br/>
<b>IT'S PROPERTIES</b>   
<br/>
    class="d-flex justify-start"    // This is how we use   
    <br/>
    other Properties- start (browser default), end, center, space-between, or space-around   
    <br/>
   <b>FLEX RESPONSIVE</b> 
    <br/>
There are also responsive variations for justify-content.   
<br/>
.justify-start   <br/>
.justify-end   <br/>
.justify-center   <br/>
.justify-space-between   <br/>
.justify-space-around   <br/>
.justify-sm-start   <br/>
.justify-sm-end   <br/>
.justify-sm-center   <br/>
.justify-sm-space-between   <br/>
.justify-sm-space-around   <br/>
.justify-md-start   <br/>
.justify-md-end   <br/>
.justify-md-center   <br/>
.justify-md-space-between   <br/>
.justify-md-space-around   <br/>
.justify-lg-start   <br/>
.justify-lg-end   <br/>
.justify-lg-center   <br/>
.justify-lg-space-between   <br/>
.justify-lg-space-around   <br/>
.justify-xl-start   <br/>
.justify-xl-end   <br/>
.justify-xl-center   <br/>
.justify-xl-space-between   <br/>
.justify-xl-space-around   <br/>

</p>

<br/>
<hr/>
<br/>

<h3>FLEX ALIGN</h3>
<p>
  When using flex align with IE11 you will need to set an explicit height as min-height will not suffice and cause undesired results.

<br/>

Choose from start, end, center, baseline, or stretch (browser default)   
<br/>
class="d-flex align-start"   // This is how we use   
<br/>
There are also responsive variations for align-items.   
<br/>

    .align-start   <br/>
    .align-end   <br/>
    .align-center   <br/>
    .align-baseline   <br/>
    .align-stretch   <br/>
    .align-sm-start   <br/>
    .align-sm-end   <br/>
    .align-sm-center   <br/>
    .align-sm-baseline   <br/>
    .align-sm-stretch   <br/>
    .align-md-start   <br/>
    .align-md-end   <br/>
    .align-md-center   <br/>
    .align-md-baseline   <br/>
    .align-md-stretch   <br/>
    .align-lg-start   <br/>
    .align-lg-end   <br/>
    .align-lg-center   <br/>
    .align-lg-baseline   <br/>
    .align-lg-stretch   <br/>
    .align-xl-start   <br/>
    .align-xl-end   <br/>
    .align-xl-center   <br/>
    .align-xl-baseline <br/>
    .align-xl-stretch <br/>

</p>

<br/>
<hr/>
<br/>

<h3>FLEX WRAP</h3>
<p>
  By default .d-flex does not provide any wrapping (behaves similarly to flex-wrap: nowrap).   
  <br/>
.flex-nowrap   <br/>
.flex-wrap   <br/>
.flex-wrap-reverse   <br/>

<br/>

These helper classes can also be applied in the format flex-{breakpoint}-{condition} to create more responsive variations based on breakpoints. The following combinations are available:
<br/>

    .flex-sm-nowrap   <br/>
    .flex-sm-wrap   <br/>
    .flex-sm-wrap-reverse   <br/>
    .flex-md-nowrap   <br/>
    .flex-md-wrap   <br/>
    .flex-md-wrap-reverse   <br/>
    .flex-lg-nowrap   <br/>
    .flex-lg-wrap   <br/>
    .flex-lg-wrap-reverse   <br/>
    .flex-xl-nowrap   <br/>
    .flex-xl-wrap   <br/>
    .flex-xl-wrap-reverse   <br/>

</p>

<br/>
<hr/>
<br/>

<h3>FLEX GROW & SHRINK</h3>
<p>
  The condition grow will permit an element to grow to fill available space, whereas shrink will permit an element to shrink down to only the space needs for its contents.
    
    <br/>

    Where condition can be either grow or shrink and value can be either 0 or 1.   
    
    <br/>
    
    flex-grow-0   <br/>
    flex-grow-1  <br/>
    flex-shrink-0   <br/>
    flex-shrink-1   <br/>

    <br/>    

These helper classes can also be applied in the format flex-{breakpoint}-{condition}-{state} to create more responsive variations based on breakpoints. The following combinations are available:

<br/>

flex-sm-grow-0  <br/>
flex-md-grow-0   <br/>
flex-lg-grow-0   <br/>
flex-xl-grow-0   <br/>
flex-sm-grow-1   <br/>
flex-md-grow-1   <br/>
flex-lg-grow-1   <br/>
flex-xl-grow-1   <br/>
flex-sm-shrink-0   <br/>
flex-md-shrink-0   <br/>
flex-lg-shrink-0   <br/>
flex-xl-shrink-0   <br/>
flex-sm-shrink-1   <br/>
flex-md-shrink-1   <br/>
flex-lg-shrink-1   <br/>
flex-xl-shrink-1       <br/>

</p>

<br/>
<hr/>
<br/>

<h3>FLOAT</h3>
<p>
  Applies a custom float across any breakpoint with responsive float utilities.
<br/>
class="float-left"  // This is how we use
<br/>
Here is a list of all the available support classes:

<br/>

    .float-left   <br/>
    .float-right   <br/>
    .float-start   <br/>
    .float-end   <br/>
    .float-none   <br/>
    .float-sm-left   <br/>
    .float-sm-right   <br/>
    .float-sm-start   <br/>
    .float-sm-end   <br/>
    .float-sm-none   <br/>
    .float-md-left   <br/>
    .float-md-right   <br/>
    .float-md-start   <br/>
    .float-md-end   <br/>
    .float-md-none   <br/>
    .float-lg-left   <br/>
    .float-lg-right   <br/>
    .float-lg-start   <br/>
    .float-lg-end   <br/>
    .float-lg-none   <br/>
    .float-xl-left   <br/>
    .float-xl-right   <br/>
    .float-xl-start   <br/>
    .float-xl-end   <br/>
    .float-xl-none   <br/>

</p>

<br/>
<hr/>
<br/>


<span class="text-h1">Hello</span>
</div>
</template>

<script>
export default{
    name:"AllcompNotes",

}
</script>

<style>
</style>