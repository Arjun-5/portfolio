---
title: Contact Me
layout: Contact_Me
nav-menu: true
---

<div id="main">
<section id="one">	
	<section id="contact">
		<div class="inner">
			<section style="margin-left:15px;">
				<form action="https://formspree.io/f/xnqydpyl" target="receiver" method="POST">
				<div class="field half first">
					<label for="name" style="color: #cfc9c2; font-family: 'Cooper Black';">Name</label>
					<input type="text" name="name" id="name" style="color: #f7768e; font-family: 'Perpetua'; font-size:22px" required/>
				</div>
				<div class="field half">
					<label for="email" style="color: #cfc9c2; font-family: 'Cooper Black';">Email</label>
					<input type="text" name="_replyto" id="email" style="color: #f7768e; font-family: 'Perpetua'; font-size:22px" required/>
				</div>
				<div class="field">
					<label for="message" style="color: #cfc9c2; font-family: 'Cooper Black';">Message</label>
					<textarea name="message" id="message" rows="6" style="color: #f7768e; font-family: 'Perpetua'; font-size:22px" required></textarea>
				</div>
				<ul class="actions">
					<li><input type="submit" value="Send Message" style="color: #1a1b26; font-family: 'Perpetua'; font-size:20px" class="special" onClick="urlChange()"/></li>
					<li><input type="reset" value="Clear" style="color: #cfc9c2; font-family: 'Perpetua'; font-size:20px" /></li>
				</ul>
				</form>
				<div class="iframebox">
				<iframe class="responsive-iframe" name="receiver" id="receiver"	></iframe>
				</div>
			</section>
			<section class="split">
			<section>
				<div class="contact-method">
					<span class="icon alt fa-envelope"></span>
					<h3 style="color: #cfc9c2; font-family: 'Cooper Black';">Email</h3>
					<a href="#" style="color: #f7768e; font-family: 'Perpetua'; font-size:28px">{{ site.email }}</a>
				</div>
			</section>
			<section>
				<div class="contact-method">
					<span class="icon alt fa-phone"></span>
					<h3 style="color: #cfc9c2; font-family: 'Cooper Black';">Phone</h3>
					<span style="color: #f7768e; font-family: 'Perpetua'; font-size:28px">{{ site.phone }}</span>
				</div>
			</section>
			<section>
				<div class="contact-method">
					<span class="icon alt fa-home"></span>
					<h3 style="color: #cfc9c2; font-family: 'Cooper Black';">Address</h3>
					<span style="color: #f7768e; font-family: 'Perpetua'; font-size:28px">
					{% if site.street_address %}
					    {{ site.street_address }}<br />
					{% endif %}
					{% if site.city %}
					    {{ site.city }},
					{% endif %}
					{% if site.state %}
					    {{ site.state }} 
					{% endif %}
					{% if site.zip_code %}
					    {{ site.zip_code }}<br />
					{% endif %}
					{% if site.country %}
					    {{ site.country }}
					{% endif %}
					</span>
				</div>
			</section>
		</section>
	</div>
</section>
</section>
</div>
