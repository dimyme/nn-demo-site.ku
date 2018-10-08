Always wanted to run a website on your own domain for free ?

This is a demo example   http://www.nn-demo-site.ku/ , listed at  http://new-nations.net/tld/ku  to show how to achieve this feat. We are using:

* the free github-pages to host stuff
* https://blockchain-dns.info   add-on so firefox can actually surf to  a  \*.ku  website
* this guy claims he has done it too:    http://albino.cyb 



.../docs/ is the actual hmtl file  directory   to be hosted on    http://nn-demo-site.ku  via github-pages for free

instead of static html, we use those templates by github

This is to demonstrate how it can be done, since it involves some DNS trickery which no one bothered to document anywhere near.

setting things up on the cheap (i.e. not using our own DNS server called "knot-resolver" kresd / knotr) is done right quick:

 * on NN, 
register a subdomain  such as   thisISMYown.ku

and configure it like so:


  * configure nn-demo-site.ku

nn-demo-site.ku to IP Address (address of your web server)

Enter IP Address (e.g. www.nn-demo-site.ku = 123.213.14.105 )

http://www.nn-demo-site.ku = 123.213.14.105


    123.213.14.105 seems to be the NN DNS or something.








     
 * gh tells us:

Setting up an apex domain

To set up an apex domain, such as example.com, you must configure an ALIAS, ANAME, or A record with your DNS provider.

Setting up a www subdomain

To set up a www subdomain, such as www.example.com you must configure a CNAME record with your DNS provider.




 * github project settings
 
the gh-pages setup just need on special setting, namely "custom domain" set to  ''nn-demo-site.ku''
    
    
    done !    

actually, that's it. the .ku page displays handsomely. There is an error msg because of .ku, but we just ignore it since it works well regardless.

now how to use our local knot-resolver slave-zone ?

Also, using an openNIC domain gives us more control than New-Nations. With openNIC we have more DNS records to manipulate.  







