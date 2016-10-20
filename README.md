# Integrate PHP Dynamic AntiAdblock Ads to Symfony2 & 3
This is an example of twig extension that you can integrate to symfony2 project to ad ads. What you need to change is the file AntiAdblockExtension.php

      /** @var string */
    private $token = 'YOUR_TOKEN';
    /** @var int */
    private $zoneId = 'ZONE Id';
    
Create an adzone to get those values

# Calling the extension:
Just add this line to your twig view to render the javascript code
   
    {{ 'ads'|showAds()|raw }}
