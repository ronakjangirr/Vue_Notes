<template>

<div>

    <h2>Alingments</h2>

    <div class="d-sm-none d-md-flex">
            <h1 class="text-center yellow--text">Div 1
            </h1>
            <p>Note- d-sm-none => Small to medium tablet Hide in Between (600px to 960px) if we use with (d-md-flex)
                otherwise it will hide in other all properties like (md,lg, xl, xxl) </p>
        </div>

        <div class="d-md-none d-lg-flex">
            <h1 class="text-center blue--text">Div 2</h1>
            <p>Note- d-md-none => Medium md Large tablet to laptop (960px to 1280px) if we use with (d-lg-flex) otherwise it
                will hide in other all properties like (lg, xl, xxl) </p>
        </div>

        <div class="d-lg-none d-xl-flex">
            <h1 class="text-center red--text">Div 3</h1>
            <p>Note- d-lg-none => Large lg Laptop to desktop (1280px to 1920px) if we use with (d-xl-flex) otherwise it will
                hide in other all properties like (xl, xxl) </p>
        </div>

        
<br />
<hr />
<br />


<v-container style="height: 500px; border: 1px solid #ccc; width: 500px" class="d-flex flex-row">
    <v-row>
        <v-col>
            <h2>Div 1</h2>
        </v-col>
        <v-col>
            <h2>Div 2</h2>
        </v-col>
        <v-col>
            <h2>Div 3</h2>
        </v-col>
    </v-row>
</v-container>

<br />
    <hr />
<br />

<ul>Without using d-flex</ul>

<div class="parent-style">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />


<ul>1.use d-flex for applying the properties flex</ul>

<div class="parent-style d-flex">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>

</div>

<br />
    <hr />
<br />

<ul>flex-column</ul>
<div class="parent-style d-flex flex-column">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />

<ul>justify-start</ul>
<div class="parent-style d-flex justify-start">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />

<ul>justify-end</ul>
<div class="parent-style d-flex justify-end">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />

<ul>justify-center</ul>
<div class="parent-style d-flex justify-center">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />


<ul>justify-space-between</ul>
<div class="parent-style d-flex justify-space-between">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />

<ul>justify-space-around</ul>
<div class="parent-style d-flex justify-space-around">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />

<ul>justify-sm-center- Only Above 600px it will come in center and carry on upto xl and below 600 it will be at starting position(static)</ul>
<div class="parent-style d-flex justify-sm-center">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />

<ul>justify-md-center- Only Above 960px it will come in center and carry on upto xl and below 960 it will be at starting position(static)</ul>
<div class="parent-style d-flex justify-md-center">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />

<ul>justify-lg-center- Only Above 1264px it will come in center and carry on upto xl and below 1264px it will be at starting position(static)</ul>
<div class="parent-style d-flex justify-lg-center">
    <div class="child-style">
        <h1>Div1</h1>
    </div>
    <div class="child-style">
        <h1>Div2</h1>
    </div>
    <div class="child-style">
        <h1>Div3</h1>
    </div>
</div>

<br />
    <hr />
<br />

<ul>flex-wrap- when we apply fixed height to the parent except (height:"auto") then flex-wrap try to fit the child content in given parent div </ul>
<div class="parent2-style d-flex justify-space-around flex-wrap ">
    <div class="child2-style">
        <h1>div 1</h1>
    </div>
    <div class="child2-style">
        <h1>div 2</h1>
    </div>
    <div class="child2-style">
        <h1>div 3</h1>
    </div>
    <div class="child2-style">
        <h1>div 4</h1>
    </div>
    <div class="child2-style">
        <h1>div 5</h1>
    </div>
    <div class="child2-style">
        <h1>div 6</h1>
    </div>
</div>


<br/>
<hr/>
<br/>

<div class="parent2-style d-flex justify-space-around">
    <div class="child2-style">
        <h1>div 1</h1>
    </div>
    <div class="child2-style">
        <h1>div 2</h1>
    </div>
    <div class="child2-style">
        <h1>div 3</h1>
    </div>
    <div class="child2-style">
        <h1>div 4</h1>
    </div>
    <div class="child2-style">
        <h1>div 5</h1>
    </div>
    <div class="child2-style">
        <h1>div 6</h1>
    </div>
</div>

<br/>
<hr/>
<br/>

<ul> used d-flex & justify-space-around on (row) and used cols and applied (cols="6"  sm="4" md="3" lg="2") </ul>        

<v-container class="parent2-style">
<v-row class="d-flex justify-space-around">

<v-col cols="6"  sm="4" md="3" lg="2">

<div class="child2-style">div1</div>

</v-col>
<v-col cols="6"  sm="4" md="3" lg="2">

<div class="child2-style">div2</div>

</v-col>
<v-col cols="6"  sm="4" md="3" lg="2">

<div class="child2-style">div3</div>

</v-col>
<v-col cols="6"  sm="4" md="3" lg="2">

<div class="child2-style">div4</div>

</v-col>
<v-col cols="6"  sm="4" md="3" lg="2">

<div class="child2-style">div5</div>

</v-col>
<v-col cols="6" sm="4" md="3" lg="2">

<div class="child2-style">div6</div>

</v-col>

</v-row>
</v-container>


</div>

</template>

<script>
export default{
    name:"FlexVue"
}
</script>

<style>

.parent-style{
height:200px;
border: 1px solid black;
width: 500px;
}

.parent2-style{
height:auto;
border: 1px solid black;
width: 100%;
padding:10px;
}


.child-style{
    height: 100px; 
    border: 1px solid #ccc; 
    width: 100px;
}

.child2-style{
    height: 8rem; 
    border: 0.1rem solid #ccc; 
    width: 8rem;
    margin: 1rem;
    box-sizing: border-box;
}
</style>