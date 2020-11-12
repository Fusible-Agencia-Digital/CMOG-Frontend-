<template>
    
</template>
<script>
  export default {
    name: "payment-chat",
    layout: "chat",
    head() {
        return {
            __dangerouslyDisableSanitizers: ['script'],
            script: [
                {
                    hid: 'zoho',
                    //innerHTML: "var _smartsupp = _smartsupp || {};_smartsupp.key = 'f05d28f4332f6998dbbe2ee4832c4ce37d354e07';window.smartsupp||(function(d) {var s,c,o=smartsupp=function(){ o.push(arguments)};o=[];s=d.getElementsByTagName('script')[0];c=d.createElement('script');c.type='text/javascript';c.charset='utf-8';c.async=true;c.src='https://www.smartsuppchat.com/loader.js?';s.parentNode.insertBefore(c,s);})(document);",
                    innerHTML: 'var $zoho=$zoho || {};$zoho.salesiq = $zoho.salesiq || {widgetcode:"2151b329adbbdfc4a5baf6bd279efda8197375e5d3b0eff46912fc45ce356f2f", values:{},ready:function(){}};var d=document;s=d.createElement("script");s.type="text/javascript";s.id="zsiqscript";s.defer=true;s.src="https://salesiq.zoho.com/widget";t=d.getElementsByTagName("script")[0];t.parentNode.insertBefore(s,t);d.write("<div id=\'zsiqwidget\'></div>");',
                    type: 'text/javascript',
                    charset: 'utf-8'
                }
            ]
        }
    },

  }
</script>
