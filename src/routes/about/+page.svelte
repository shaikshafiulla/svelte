<h1>this is about page</h1>
<a href="/">home page</a>

<script>
	import { afterNavigate,beforeNavigate,goto } from "$app/navigation";


    beforeNavigate(navigation=>{
    console.log(' before navigation :>> ', navigation);
   });
   afterNavigate(navigation=>{
    console.log('after navigation :>> ', navigation);
   });
</script>