# Integrate PHP Dynamic AntiAdblock Ads to Symfony2 & 3
This is an example of twig extension that you can integrate to symfony2 website to add the PHP version of propellers ads's tag  . 
What you need to change is the lines 8 and 11 of file AntiAdblockExtension.php

      /** @var string */
    private $token = 'YOUR_TOKEN';
    /** @var int */
    private $zoneId = 'ZONE Id';
    
Create an adzone to get those values

# Calling the extension:
Just add this line to your twig view to get the javascript dynamic tag
   
    {{ 'ads'|showAds()|raw }}
