<template>
<div>
    <v-breadcrumbs
        :items="items"
        divider="-">

    </v-breadcrumbs>
</div>
</template>

<script>

export default{
    name:"BreadCrumbs",

    data: () => {
    return {
        items: [
        {
          text: 'Dashboard',
          disabled: false,
          href: 'breadcrumbs_dashboard',
        },
        {
          text: 'Link 1',
          disabled: false,
          href: 'breadcrumbs_link_1',
        },
      ],
    }
    }   

}



</script>

<style>

</style>