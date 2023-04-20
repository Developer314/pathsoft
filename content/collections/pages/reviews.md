---
id: 53d390e2-b80b-4c49-81a0-21c23dcd5ac1
blueprint: page
title: Reviews
author: 7fbe8121-f27b-4e33-8a24-834e62f76e98
template: reviews/index
breadcrumb: |-
  <nav class="bread-crumbs">
  				<div class="container">
  					<div class="row">
  						<div class="col-12">
  							<ul class="bread-crumbs-list">
  								<li>
  									<a href="/">Home</a>
  									<i class="material-icons md-18">chevron_right</i>
  								</li>
  								<li>
  									<a href="/services">Services</a>
  									<i class="material-icons md-18">chevron_right</i>
  								</li>
  								<li>Reviews</li>
  							</ul>
  						</div>
  					</div>
  				</div>
  			</nav>
meta_title: 'Your Page/Site Name'
meta_description: 'Your Page Meta Description'
meta_keywords: 'Tag 1, Tag 2'
og_title: 'OG Title'
og_description: 'OG Description'
updated_by: 7fbe8121-f27b-4e33-8a24-834e62f76e98
updated_at: 1682000413
block_types:
  -
    id: lgp7m2jf
    title_1: 'WE ARE ALWAYS IN TOUCH'
    title_2: Contacts
    title_3: 'Get in Touch'
    address: '4730 Crystal Springs Dr, Los Angeles, CA'
    phone: |-
      +1 323-913-4688
      +1 323-888-4554
    email: |-
      mail@example.com
      info@example.com
    working_hours: 'Mon - Fri: 9:00 - 18:00'
    location_map_iframe: '<iframe class="lazy" data-src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3302.1020346961877!2d-118.2916255847825!3d34.14373158058114!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x80c2c0623fe71971%3A0xc829e89a5dcc767e!2zNDczMCBDcnlzdGFsIFNwcmluZ3MgRHIsIExvcyBBbmdlbGVzLCBDQSA5MDAyNywg0KHQv9C-0LvRg9GH0LXQvdGWINCo0YLQsNGC0Lgg0JDQvNC10YDQuNC60Lg!5e0!3m2!1suk!2sua!4v1621932036298!5m2!1suk!2sua"></iframe>'
    edit_template: true
    template: |-
      <div class="section">
      				<div class="container">
      					<div class="row content-items">
      						<div class="col-12">
      							<div class="section-heading">
      								<div class="section-subheading">{{title_1}}</div>
      								<h1>{{title_2}}</h1>
      							</div>
      						</div>
      						<div class="col-xl-4 col-md-5 content-item">
      							<div class="contact-info section-bgc">
      								<h3>{{title_3}}</h3>
      								<ul class="contact-list">
      									<li>
      										<i class="material-icons material-icons-outlined md-22">location_on</i>
      										<div class="footer-contact-info">
      											{{address}}
      										</div>
      									</li>
      									<li>
      										<i class="material-icons material-icons-outlined md-22">smartphone</i>
      										<div class="footer-contact-info">
      											{{phone}}
      										</div>
      									</li>
      									<li>
      										<i class="material-icons material-icons-outlined md-22">email</i>
      										<div class="footer-contact-info">
      											{{email}}
      										</div>
      									</li>
      									<li>
      										<i class="material-icons material-icons-outlined md-22">schedule</i>
      										<div class="footer-contact-info">{{working_hours}}</div>
      									</li>
      								</ul>
      							</div>
      						</div>
      						<div class="col-xl-8 col-md-7 content-item">
      							 {{ form:contact }}
                         
                            
                            {{ if success }}
                                <div class="bg-green-300 text-white p-2">
                                    {{ success }}
                                </div>
                            {{ else }}
                               
                                {{ if errors }}
                                    <div class="bg-red-300 text-white p-2">
                                        {{ errors }}
                                            {{ value }}<br>
                                        {{ /errors }}
                                    </div>
                                {{ /if }}
                         
                              
                                {{ fields }}
                                    <div class="p-2">
                                        <label>{{ display }}</label>
                                        <div class="p-1">{{ field }}</div>
                                        {{ if error }}
                                            <p class="text-gray-500">{{ error }}</p>
                                        {{ /if }}
                                    </div>
                                {{ /fields }}
                         
                               
                                <input type="hidden" class="hidden" name="{{ honeypot ?? 'honeypot' }}">
                         
                                
                                <button type="submit" class="btn btn-w240 ripple">Submit</button>
                            {{ /if }}
                         
                        {{ /form:contact }}
      						</div>
      					</div>
      				</div>
      			</div>
      			
      			<div class="map">
      				{{location_map_iframe}}
      			</div>
    type: contact_us
    enabled: true
---
