<html>
    <body>
        <script type='text/javascript'>
        function initEmbeddedMessaging() {
            try {
                embeddedservice_bootstrap.settings.language = 'pt_BR';

                window.addEventListener("onEmbeddedMessagingReady", () => {

                    console.log("onEmbeddedMessagingReadyEUD>> ");
                });

                embeddedservice_bootstrap.init(
                    '00D3B000000IPck',
                    'CRCEudora',
                    'https://grupoboticario--uat.sandbox.my.site.com/ESWCRCEudora1700594690414',
                    {
                        scrt2URL: 'https://grupoboticario--uat.sandbox.my.salesforce-scrt.com'
                    }
                );
            } catch (err) {
                console.error('Error loading Embedded Messaging: ', err);
            }
        };
        </script>
        <script type='text/javascript' src='https://grupoboticario--uat.sandbox.my.site.com/ESWCRCEudora1700594690414/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
    </body>
</html>
