---
layout: post
title: "Basmati Rice with mushrooms in the pressure cooker"
description: "How to cook whole corn basmati rice with mushrooms in the pressure cooker"
tags: [basmati rice, pressure cooker, whole corn ]
---

How to cook 

## Cook time 30 min 
Preparation aprox 20 min
Ingredients (enough for 4 servings)
<figure>
	<a href="https://farm8.staticflickr.com/7677/26793634544_651e8c739e_z_d.jpg"><img src="https://farm8.staticflickr.com/7677/26793634544_651e8c739e_z_d.jpg" alt=""></a>
	<figcaption><a href="http://www.flickr.com/photos/80901381@N04/7758832526/" title="Ingredients">Ingredients</a>.</figcaption>
</figure>
1. Basmati rice around 200g
2. Mushrooms around 250g (I used 400g)
3. 2 small onions
4. garlic
5. 4 tbsp native oil 


Preparation
1. chop the onions
2. wash the brown rice
3. wash and chop the mushrooms in slices 

Cooking
1. heat the olive oil in the open pressure cooker
2. add the chopped onion in small pieces and fry it for 3 minutes
3. add the brown rice and fry it for a couple of minutes
4. pour double the water into the open pressure cooker and bring it to boil
5. turn the heat/fire down and let it cook for around 10 minutes (in the mean time clean and chop the mushrooms if not already did so)
6. add the mushrooms and salt now to the pressure cooker pot and stir. 
7. now lock the lid (I used level 1 - 110 degrees Celsius)
8. let it cook for another 10-15 minutes in the pressure cooker
9. do a pressure release and then let it cool
10. bon apetit   


### One Up

<figure>
	<a href="https://farm8.staticflickr.com/7401/26793751653_5494f38a28_z_d.jpg"><img src="https://farm8.staticflickr.com/7401/26793751653_5494f38a28_z_d.jpg" alt=""></a>
	<figcaption><a href="http://www.flickr.com/photos/80901381@N04/7758832526/" title="Morning Fog Emerging From Trees by A Guy Taking Pictures, on Flickr">Morning Fog Emerging From Trees by A Guy Taking Pictures, on Flickr</a>.</figcaption>
</figure>

### Two Up

Apply the `half` class like so to display two images side by side that share the same caption.

{% highlight html %}
<figure class="half">
	<img src="/images/image-filename-1.jpg" alt="">
	<img src="/images/image-filename-2.jpg" alt="">
	<figcaption>Caption describing these two images.</figcaption>
</figure>
{% endhighlight %}

And you'll get something that looks like this:

<figure class="half">
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<img src="http://placehold.it/600x300.jpg" alt="">
	<img src="http://placehold.it/600x300.jpg" alt="">
	<figcaption>Two images.</figcaption>
</figure>

### Three Up

Apply the `third` class like so to display three images side by side that share the same caption.

{% highlight html %}
<figure class="third">
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<figcaption>Caption describing these three images.</figcaption>
</figure>
{% endhighlight %}

And you'll get something that looks like this:

<figure class="third">
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<a href="http://placehold.it/1200x600.jpg"><img src="http://placehold.it/600x300.jpg" alt=""></a>
	<figcaption>Three images.</figcaption>
</figure>

### Alternative way

Another way to achieve the same result is to include `gallery` Liquid template. In this case you
don't have to write any HTML tags – just copy a small block of code, adjust the parameters (see below)
and fill the block with any number of links to images. You can mix relative and external links.

Here is the block you might want to use:

{% highlight jinja %}
{% raw %}
{% capture images %}
	/images/abstract-10.jpg
	/images/abstract-11.jpg
	http://upload.wikimedia.org/wikipedia/en/2/24/Lenna.png
{% endcapture %}
{% include gallery images=images caption="Test images" cols=3 %}
{% endraw %}
{% endhighlight %}

Parameters:

- `caption`: Sets the caption under the gallery (see `figcaption` HTML tag above);
- `cols`: Sets the number of columns of the gallery.
Available values: [1..3].

It will look something like this:

{% capture images %}
	/images/abstract-10.jpg
	/images/abstract-11.jpg
	http://upload.wikimedia.org/wikipedia/en/2/24/Lenna.png
{% endcapture %}
{% include gallery images=images caption="Test images" cols=3 %}
