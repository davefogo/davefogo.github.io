It had been a long while since I touched any Ruby code. For the past 6 months I had been completely focused on Javascript (vanilla, jQuery, Angular, Firebase). Now its time to get my Ruby shirt on. When I first started on Ruby this week again it took a while for me to get used to it. Maybe 1 hour and then I was fluid. I guess this is normal when you are not used to changing from one language to the other. This happened also to me when I was switching from Spanish to English, or Spanish to German. This time around I started with some codewars to get my mind fresh on Ruby.

A couple of neat methods I learned this week were ```swapcase``` and ```reduce```. These incredibly simple and efficient methods surprised me. swapcase takes a string and “swaps” the cases of each letter. i.e :

```
"I am a String".swapcase
 => "i AM A sTRING
 ```
 
 I had gotten to know reduce in Javascript and in Ruby it works in a similar fashion. It takes an array and runs every element agains a block of code or a symbol ( named method) and returns an accumulation of the whole. Example:
 
 ```
[1,2,3,4,5].reduce(:+)
 =>15
 ```
 
 In this case each element of the array is passed to the add method and thus it adds each element to the accumulator.
