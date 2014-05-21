![Buddycloud](images/logos/2000x2000-blue-on-white.png)



---



#State of the federated social web
Notes:
"We're all here because we believe in distributed systems and the open web.



---



##Developers have to solve some very difficult problems
<ul>
    <li class="fragment">authentication</li>
    <li class="fragment">security</li>
    <li class="fragment">cross-device synchronization</li>
    <li class="fragment">offline message management</li>
    <li class="fragment">and more</li>
</ul>



---



##feature indecision



---



##identity indecision
<span data-fragment-index="1" class="fragment current-visible">`my-personal-domain.com`</span>
<span data-fragment-index="2" class="fragment current-visible">`example.com/username`</span>
<span data-fragment-index="3" class="fragment current-visible">`username.example.com`</span>
<span data-fragment-index="4" class="fragment current-visible">`@username` and we'll ignore peering for the moment</span>
<span data-fragment-index="5" class="fragment current-visible">2dbf1ce81180d9ed9258e3e8729ba642c8ab2a31268d31cd2c7ffe8693e3a02e</span>



---



### "We'll put up and API and call it open"



---



###"Your user's profile should include these fields"
`include <long wishlist>`
* <span class="fragment">"You insensitive clod! What do you mean it won't run on my RaspberryPi?".</span>  <span class="fragment">256MB</span>



---



###"what do you mean you don't include semantic web markup?"
<span class="fragment">(we like the semantic web)</span>



---



###Frankly we don't have a clue what apps people will build. 
###Each person has their own view of a solution.



---



##push innovation to the edge#

* right tools 
* in the right hands
* (with good docs)

Notes:
- Push innovation to the edge (this has been true through history)



---



###we have been doing it all wrong 

<span data-fragment-index="1" class="fragment">build a federated social network</span>

<span data-fragment-index="2" class="fragment">build developers tools (that just happen to be federated)</span>

<span data-fragment-index="3" class="fragment">(Stealth Federation - Alex Feyerke)</span>



---



##We need building blocks



---



###We came up with a plan
<ul>
    <li class="fragment">time pressure</li>
    <li class="fragment">security and encryption concerns</li>
    <li class="fragment">lack of a framework to just drop in</li>
    <li class="fragment">complexity</li>
    <li class="fragment">not sure what libraries to use</li>
    <li class="fragment">not sure about how to do realtime or push</li>
</ul>



---



##and built a solution



---



##Unix approach
- Small is beautiful.
- Make each program do one thing well.
- Build a prototype as soon as possible.
- Choose portability over efficiency.



---



##Simple ID

`username@example.com`



---



##Used XMPP's federation layer



---



##Defined a common language / protocol / XEP



---



##non-judgemental federateration

* run it yourself 
* get hosted + migrate your data later
* don't federate




---



##easy to extend
* fork the open source code
* mix-and-match components
* extend components
* extend data types
* extend data location



---



##Build using components
* server process
* interconnect using TCP
* interconnect with local and remote servers



---



###Buddycloud is a set of federated building blocks that can be mixed and matched, and extended



---



##Buddycloud components
* channel server
* media server
* friend finder
* HTTP api server
* XMPP-ftw(-buddycloud)
* push notifications
* content and channel search
* recommender
* nearby search



---



<!-- .slide: data-background="#fff" data-state="hide-all-controls"  -->
![Buddycloud](images/logos/architecture-diagram.png)



---



##...and third-party integrations
* github
* jenkins



---



##Channels
* `user@example.com`
* `user@example.com/posts`
* `user@example.com/to-do_list`
* `user@example.com/geo-location`
* `user@example.com/bookmarks`



---



<!-- .slide: data-background="#fff" data-state="hide-all-controls"  -->
```
{
    "id": "94abf702-fd32-4351-b955-8f9613bf1844",
    "entry": {
      "atom": {
        "title": "Post",
        "id": "tag:null@channels.buddycloud.org,/user/simon@buddycloud.org/posts,94abf702-fd32-4351-b955-8f9613bf1844",
        "updated": "2014-04-25T08:48:43.410Z",
        "published": "2014-04-25T08:48:43.410Z",
        "content": {
          "content": "I really need a http://laughingsquid.com/catable-a-sleek-modern-desk-hiding-a-bevy-of-hidey-holes-to-please-hardworking-humans-and-curious-cats-alike/ ",
          "type": "text"
        },
        "author": {
          "name": "simon@buddycloud.org",
          "uri": "acct:simon@buddycloud.org"
        }
      },
      "activity": {
        "verb": "post",
        "object": {
          "object-type": "note"
        },
        "author": {
          "object-type": "person"
        }
      }
    },
    "node": "/user/simon@buddycloud.org/posts"
  },
```



---



<!-- .slide: data-background="#fff" data-state="hide-all-controls"  -->
![What is a channel?](images/logos/publish-subscribe.png)



---



<!-- .slide: data-background="#fff" data-state="hide-all-controls"  -->
![Publish Subscribe](images/logos/channel-hierachy.png)



---



###Demo
* Show posting
* Show media



---



###Long term goals
* Chaortic leadership
* 30 year goal



---



###Next steps
* hosting.buddycloud.com
* github.com/buddycloud
* @buddycloud



---



<!-- .slide: data-background="#000" data-state="hide-all-controls"  -->
# The End <span class="fragment">?</span>




---



## Notes Slide

This slide has some notes. Hit s.

Notes:
- Note 1
- Note 2
- Notes and notes and notes.



---



## Vertical slide



--



## Vertical slide 2



---



## **JS** is cool

```javascript
// comment
var x = 100,
    y = ['a', 100, {}],
    z = {
        x: 'z'
    };
// IIFE
(function ($, window, undefined) {
    // What am I doing?
    var _test = function () {};
    return {
        test: _test
    };
})(jQuery, window)
```



---



## Slide Heading
### Sub Heading

Some text. *Italic.* **Bold.**



---



<h1 class="big">Big **Title** Slide</h1>



---



## Bulleted Fragment List

<ul>
    <li class="fragment">This is a <span>thing</span></li>
    <li class="fragment">This is <span>thing</span> thing</li>
    <li class="fragment">Thing <span>3</span></li>
</ul>



---



## Simultaneous Fragments


<span data-fragment-index="1" class="fragment current-visible">One</span>
<span data-fragment-index="2" class="fragment current-visible">at</span>
<span data-fragment-index="3" class="fragment current-visible">a</span>
<span data-fragment-index="4" class="fragment current-visible">time</span>



---



## Slide with an image

![img](images/andbang.png)



---



## More slides

> This is a blockqoute!  
> Line 2  
> <small>Luke?</small>



---



<!-- .slide: data-background="#000" data-state="hide-all-controls"  -->
# The End <span class="fragment">?</span>



---



<!-- .slide: data-background="#000" -->
# &nbsp;






