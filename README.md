**Depreciated!**

No longer functional due to changes on the Dell site. With a colleague we've updated this to Python for a 2nd version. This will be uploaded soon.

===

# Dell Database Query

Perl script to query the Dell DB to look up purchase dates

In my company, we have thousands of Dell PC's across nearly 70 sites. Our IT team tracks them in one way, and our Finance team tracks them in another. This script is useful to me because it combines what both teams need, and I can easily calculate the asset expiration date and do future planning for myself.

This script is pretty simple, and was written to avoid needing to look up each service tag from [Dell Support](http://www.dell.com/support/home/us/en/19) one-by-one, as well as to avoid having to enter a CAPTCHA each time.

How it works:

1. Collect all of your service tags into a single .txt file (ex: FPDN5Z1)
2. Edit line 8 *(my $inputfile = "")* to the name of your .txt with the service tags in it
3. Edit line 11 *(my $outputfile = "")* to the name of the .txt you want the output to be in
4. Make sure you have [Perl](https://www.perl.org/get.html) installed
5. Run the script from the directory you have it in: **perl dellquery.pl**

The resulting output .txt will be in the same directory as your input .txt

Best results come from when the Perl script, input .txt and output .txt are all in the same directory.
