---
id: home
blueprint: pages
title: Home
template: home
author: 7fbe8121-f27b-4e33-8a24-834e62f76e98
updated_by: 7fbe8121-f27b-4e33-8a24-834e62f76e98
updated_at: 1682002075
meta_title: 'Your Page/Site Name'
meta_description: 'Your Page Meta Description'
meta_keywords: 'Tag 1, Tag 2'
og_title: 'OG Title'
og_description: 'OG Description'
block_types:
  -
    id: lgooa8rn
    title_1: Welcome
    title_2: 'Lorem Ipsum'
    description: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book."
    background: intro-img1.jpg
    button_1_text: 'Learn More'
    button_1_link: 'entry::home'
    button_1_target: _self
    button_2_text: 'Contact Us'
    button_2_link: 'entry::home'
    button_2_target: _self
    edit_template: true
    template: |-
      <div class="section-bgc intro">
      				<div class="intro-item intro-item-type-1" style="background-image: url('{{background}}');">
      					<div class="container">
      						<div class="row">
      							<div class="col">
      								<div class="intro-content" style="--margin-left: 4rem;">
      									<div class="section-heading shm-none">
      										<div class="section-subheading">{{title_1}}</div>
      										<h1>{{title_2}}</h1>
      										<p class="section-desc">{{description}}</p>
      									</div>
      									<div class="btn-group intro-btns">
      										<a href="{{button_1_link}}" target="{{button_1_target}}" class="btn btn-border btn-with-icon btn-small ripple">
      											<span>{{button_1_text}}</span>
      											<svg class="btn-icon-right" viewBox="0 0 13 9" width="13" height="9"><use xlink:href="assets/img/sprite.svg#arrow-right"></use></svg>
      										</a>
      										<a href="{{button_2_link}}" target="{{button_2_target}}" class="btn btn-border btn-with-icon btn-small ripple">
      											<span>{{button_2_text}}</span>
      											<svg class="btn-icon-right" viewBox="0 0 13 9" width="13" height="9"><use xlink:href="assets/img/sprite.svg#arrow-right"></use></svg>
      										</a>
      									</div>
      								</div>
      							</div>
      						</div>
      					</div>
      				</div>
      			</div>
    type: home_hero
    enabled: true
  -
    id: lgovey7c
    title_1: 'AREAS WHAT WE SERV'
    title_2: 'Our Services'
    button_text: 'See All Services'
    service_page: 'entry::b4a26919-5ffd-4a28-904c-838b9ff38e34'
    edit_template: true
    template: |-
      <section class="section">
      				<div class="container">
      					<div class="row">
      						<header class="col-12">
      							<div class="section-heading heading-center">
      								<div class="section-subheading">{{title_1}}</div>
      								<h2>{{title_2}}</h2>
      							</div>
      						</header>
      												
      						{{collection:our_service limit="3"}}
      						<div class="col-lg-4 col-md-12 col-12 item">
      							<a href="{{url}}" class="iitem item-style iitem-hover">
      								<div class="iitem-icon">
      									<i class="material-icons material-icons-outlined md-48">{{icon}}</i>
      								</div>
      								<div class="iitem-icon-bg">
      									<i class="material-icons material-icons-outlined">{{icon}}</i>
      								</div>
      								<h3 class="iitem-heading item-heading-large">{{title}}</h3>
      								<div class="iitem-desc">{{short_description}}</div>
      							</a>
      						</div>
      						{{/collection:our_service}}
      						
      						
      						<div class="section-footer col-12 section-footer-animate">
      							<div class="btn-group align-items-center justify-content-center">
      								<a href="{{service_page}}" class="btn btn-with-icon btn-w240 ripple">
      									<span>{{button_text}}</span>
      									<svg class="btn-icon-right" viewBox="0 0 13 9" width="13" height="9"><use xlink:href="/pathsoft/assets/img/sprite.svg#arrow-right"></use></svg>
      								</a>
      							</div>
      						</div>
      					</div>
      				</div>
      			</section>
    type: our_services
    enabled: true
  -
    id: lgowb8mm
    title_1: 'SOME REASONS'
    title_2: 'Why Choose Us'
    reasons:
      -
        id: lgowbd2l
        serial_number: '01'
        title: 'High Quality <br> Hardware'
        data: 'We use top-notch hardware to develop the most efficient apps for our customers'
      -
        id: lgowbo8h
        serial_number: '02'
        title: 'Dedicated 24\7  <br />Support'
        data: 'You can rely on our 24/7 tech support that will gladly solve any app issue you may have.'
      -
        id: lgowcd3h
        serial_number: '03'
        title: '30-Day Money-back <br /> Guarantee'
        data: 'If you are not satisfied with our apps, we will return your money in the first 30 days.'
      -
        id: lgowczgt
        serial_number: '04'
        title: 'Agile and Fast <br /> Working Style'
        data: 'This type of approach to our work helps our specialists to quickly develop better apps.'
      -
        id: lgowdoez
        serial_number: '05'
        title: 'Some Apps <br >are Free'
        data: 'We also develop free apps that can be downloaded online without any payments.'
      -
        id: lgoweary
        serial_number: '06'
        title: 'High Level of <br > Usability'
        data: 'All our products have high usability allowing users to easily operate the apps.'
    edit_template: true
    template: |-
      <section class="section section-bgc">
      				<div class="container">
      					<div class="row litems">
      						<header class="col-12">
      							<div class="section-heading heading-center">
      								<div class="section-subheading">{{title_1}}</div>
      								<h2>{{title_2}}</h2>
      							</div> 
      						</header>
      						
      						{{reasons}}
      						<div class="col-lg-4 col-md-6 col-12 litem">
      							<div class="ini">
      								<div class="ini-count">{{serial_number}}</div>
      								<div class="ini-info">
      									<h3 class="ini-heading item-heading-large">{{title}}</h3>
      									<div class="ini-desc">
      										<p>{{data}}</p>
      									</div>
      								</div>
      							</div>
      						</div>
      						{{/reasons}}
      					</div>
      				</div>
      			</section>
    type: why_choose_us
    enabled: true
  -
    id: lgowsasa
    achievements:
      -
        id: lgowsdg7
        icon: chat
        title: 'Years Of Experience'
        field_value: '10'
      -
        id: lgowsk8u
        icon: history
        title: Consultans
        field_value: '40'
      -
        id: lgowsq5p
        icon: assignment_ind
        title: Employers
        field_value: '160'
      -
        id: lgowt2n5
        icon: phonelink_setup
        title: 'Apps Developed'
        field_value: '200'
    edit_template: false
    template: |-
      <section class="section section-without-padding-bottom">
      				<div class="container">
      					<div class="row items spincrement-container">
      						{{achievements}}
      						<div class="col-xl-3 col-md-6 col-12 item">
      							<div class="counter-min">
      								<div class="counter-min-block">
      									<div class="counter-min-ico">
      										<i class="material-icons material-icons-outlined md-36">{{icon}}</i>
      									</div>
      									<div class="counter-min-numb spincrement" data-from="0" data-to="{{field_value}}">0</div>
      								</div>
      								<div class="counter-min-info">
      									<h4 class="counter-min-heading">{{title}}</h4>
      								</div>
      							</div>
      						</div>
      						{{/achievements}}
      					</div>
      				</div>
      			</section>
    type: achievements
    enabled: true
  -
    id: lgoxobw3
    title_1: 'REVIEWS FROM OUR CLIENTS'
    title_2: 'What People Say'
    button_text: 'See All Reviews'
    button_link: 'entry::53d390e2-b80b-4c49-81a0-21c23dcd5ac1'
    edit_template: true
    template: |-
      <section class="section">
      				<div class="container">
      					<div class="row">
      						<header class="col-12">
      							<div class="section-heading heading-center">
      								<div class="section-subheading">{{title_1}}</div>
      								<h2>{{title_2}}</h2>
      							</div> 
      						</header>
      						
      						
      						{{collection:reviews limit="3"}}
      						<div class="col-lg-4 col-md-6 col-12 item">
      							<div class="reviews-item item-style">
      								<div class="reviews-item-header">
      									<div class="reviews-item-img">
      										<img data-src="{{image}}" class="img-cover lazy" src="{{image}}" alt="{{title}}">
      									</div>
      									<div class="reviews-item-info">
      										<h4 class="reviews-item-name item-heading">{{title}}</h4>
      										<div class="reviews-item-position">{{sub_title}}</div>
      									</div>
      								</div>
      								<div class="reviews-item-text">
      									{{content}}
      								</div>
      							</div>
      						</div>
      						{{/collection:reviews}}
      						<footer class="section-footer col-12 section-footer-animate">
      							<div class="btn-group align-items-center justify-content-center">
      								<a href="{{button_link}}" class="btn btn-with-icon btn-w240 ripple">
      									<span>{{button_text}}</span>
      									<svg class="btn-icon-right" viewBox="0 0 13 9" width="13" height="9"><use xlink:href="/pathsoft/assets/img/sprite.svg#arrow-right"></use></svg>
      								</a>
      							</div>
      						</footer>
      					</div>
      				</div>
      			</section>
    type: reviews
    enabled: true
  -
    id: lgp8ktz2
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
    edit_template: false
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
  -
    id: lgp67dix
    title_1: 'MORE INFO ABOUT'
    title_2: 'Latest News'
    button_text: 'See All News'
    button_link: 'entry::c547b8e4-3a77-4238-a1b2-3e8a53f5e756'
    edit_template: true
    template: |-
      <section class="section section-bgc">
      				<div class="container">
      					<div class="row items">
      						<header class="col-12">
      							<div class="section-heading heading-center">
      								<div class="section-subheading">{{title_1}}</div>
      								<h2>{{title_2}}</h2>
      							</div> 
      						</header>
      						
      						{{collection:news limit="3"}}
      						<div class="col-lg-4 col-md-6 col-12 item">
      							<article class="news-item item-style">
      								<a href="{{url}}" class="news-item-img el">
      									<img data-src="{{thumbnail}}" class="lazy" src="{{thumbnail}}" alt="{{title}}">
      								</a>
      								<div class="news-item-info">
      									<div class="news-item-date">{{news_date}}</div>
      									<h3 class="news-item-heading item-heading">
      										<a href="{{url}}" title="Benefits Of Async/Await">{{title}}</a>
      									</h3>
      									<div class="news-item-desc">
      										<p>{{short_description}}</p>
      									</div>
      								</div>
      							</article>
      						</div>
      						{{/collection:news}}
      						<footer class="section-footer col-12 item section-footer-animate">
      							<div class="btn-group align-items-center justify-content-center">
      								<a href="{{button_link}}" class="btn btn-with-icon btn-w240 ripple">
      									<span>{{button_text}}</span>
      									<svg class="btn-icon-right" viewBox="0 0 13 9" width="13" height="9"><use xlink:href="/pathsoft/assets/img/sprite.svg#arrow-right"></use></svg>
      								</a>
      							</div>
      						</footer>
      					</div>
      				</div>
      			</section>
    type: latest_news
    enabled: true
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
  								<li>Corporate Solutions</li>
  							</ul>
  						</div>
  					</div>
  				</div>
  			</nav>
---
