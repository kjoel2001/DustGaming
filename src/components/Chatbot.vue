<template>
    
</template>
<script>

export default {
    method: {
        
    },
    mounted(){

    (function(d, m){
        var kommunicateSettings = 
            {"appId":"2a72b7f57d45bd4f6a5998196cad2450b","popupWidget":true,"automaticChatOpenOnNavigation":true};
        var s = document.createElement("script"); s.type = "text/javascript"; s.async = true;
        s.src = "https://widget.kommunicate.io/v2/kommunicate.app";
        var h = document.getElementsByTagName("head")[0]; h.appendChild(s);
        window.kommunicate = m; m._globals = kommunicateSettings;
    })(document, window.kommunicate || {});

    }
}
</script>
<style>

</style>
