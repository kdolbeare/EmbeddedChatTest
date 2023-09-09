<html>
  <body>
     <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			
			window.addEventListener("onEmbeddedMessagingReady", () => {            
			console.log( "Inside Prechat API!!" );
			embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( { "MCID" : "102066671" } );
		});
			embeddedservice_bootstrap.init(
				'00D7j0000004g63',
				'IRE_Chat',
				'https://remax--uat.sandbox.my.site.com/ESWIREChat1694022628525',
				{
					scrt2URL: 'https://remax--uat.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://remax--uat.sandbox.my.site.com/ESWIREChat1694022628525/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
  
    <script>
        console.log("My origin:", window.location.origin);
      </script>
  </body> 
</html>
