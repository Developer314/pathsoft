---
id: b4a26919-5ffd-4a28-904c-838b9ff38e34
blueprint: page
title: Services
author: 7fbe8121-f27b-4e33-8a24-834e62f76e98
template: our_service/index
meta_title: 'Your Page/Site Name'
meta_description: 'Your Page Meta Description'
meta_keywords: 'Tag 1, Tag 2'
og_title: 'OG Title'
og_description: 'OG Description'
updated_by: 7fbe8121-f27b-4e33-8a24-834e62f76e98
updated_at: 1682000447
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
  								
  							</ul>
  						</div>
  					</div>
  				</div>
  			</nav>
block_types:
  -
    id: lgp7mrqx
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
---
