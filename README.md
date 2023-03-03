Regex For Email Address Validation

A regex or a regular expression or a rational expression is a sequence of characters that specify a search pattern in text. These regular expressions can be a combination of numbers, letters and special characters.

I’ll be showing and going into detail about the regular expression components used to validate an email address. The code we will be going in depth about is as follows    /^w+[+.w-]*@([w-]+.)*w+[w-]*.([a-z]{2,4}|d+)$/i

Anchors
The anchors used for this regex code are ^ at the start and $ for the finish

Quantifiers
In the example regex code above we used + quite a few times. This along with the {2,4} are examples of greedy quantifiers. The {2,4} specifies that the input needs to be a minimum of 2 characters but no more than 4.

Character Classes
In this regex code there is a class of \w

Grouping and Capturing
There are three groups in our example, the first of which is /^w+[+.w-]*@. This captures everything before the @ and is our “Username”. Our second group we have in our example is ([w-]+.)*w+[w-]*. This gets everything between the @ and the . and is our domain name. The third group we have is ([a-z]{2,4}|d+)$/ this gets everything after the . and is known as the extensions.

Greedy and Lazy Match
In the example above, we only have the greedy matches + and {}. This means that the match can expand as long as it needs to.

Bracket Expressions
We have four separate bracket expressions. The information inside the [] identities which information is matched.

Author
My name is Cayson Bond and my GitHub can be found here https://github.com/C-Bond21
