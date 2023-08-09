<script>
    import {afterNavigate,beforeNavigate,goto} from "$app/navigation"
    import   ProductHeader  from "./ProductHeader.svelte"
   import {page,navigating} from "$app/stores";

    $:console.log('navigating :>> ', $navigating);

//    beforeNavigate(navigation=>{
//     console.log('navigation :>> ', navigation);
//    });
//    afterNavigate(navigation=>{
//     console.log('navigation :>> ', navigation);
//    });
</script>
<ProductHeader />
<h1> the id of the product is {$page.params.id}</h1>
<a href="/">home</a>
<button on:click={()=> goto('/')}>goto home page</button>