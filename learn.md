
[Page "This is a default content"]

Ok so here you are. You want to show the world how you made this awesome open source project or maybe want to
explain how it works, or maybe want to tell something else about it.


### This is the place to do it.

![Codeilm](https://codeilm.com/static/images/logo/codeilmbanner.png "Codeilm.com")

Describe your process in making this.

1. You can use, what we call **Pages** to describe each step.
2. You use Markdown for writing your content. Here is [a cheat sheet for you](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).


If you are *not sure* of how it will appear in the post. Click on the **Preview** button on the toolbar to see the magic.



```python
def user_logged_out_receiver(sender, user, request, **kwargs):
	cart = request.session.get('products',None)
	user = request.user
	print Cart.objects.filter(user=user)
	for j in Cart.objects.filter(user=user) :
		j.delete()

	print Cart.objects.all()

	if cart :
		for i in cart :
			x = ProductDescription.objects.filter(id=i).first()
			Cart.objects.create(user=user,products=x)

	request.session.clear()


user_logged_out.connect(user_logged_out_receiver)
```
[\Page]

