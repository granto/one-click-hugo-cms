---
title: The Spreadsheets
image: /img/undraw_all_the_data_h4ki.svg
heading: What we offer
description: 'Learn whether a rental property is a good investment. '
intro:
  blurbs: []
  heading: What we offer
  description: >-
    Use the tools of successful real estate investors to evaluate rental
    properties.  Our spreadsheets crunch all the numbers to show you whether the
    property is a good investment.
main:
  heading: 'Investment Property Evaluation Spreadsheet: Single Property Edition'
  description: >-
    This spreadsheet calculates the metrics needed to assess the attractiveness
    of a particular investment property. You'll see your CapRate, Cash Flow,
    Gross Rental Yield, date of cash flow positive, IRR, and other important
    metrics.  A number of premium versions will be available soon including
    Multiple Property Edition: This spreadsheet expands on the Single Property
    Edition by allowing you to compare multiple properties to see which one is
    best.
  image1:
    alt: Single property edition
    image: /img/undraw_investing_7u74.svg
  image2:
    alt: Multiple property edition
    image: /img/undraw_city_girl_ccpd.svg
testimonials: []
pricing:
  heading: Monthly subscriptions
  description: >-
    Get access to your own version where you can save your inputs and receive
    access to updates and get support.
  plans:
    - description: >-
        Perfect for those evaluating a single property or looking to better
        understand their current property.
      items:
        - ''
      plan: Single Property Edition
      price: '20'
      <!-- Load Stripe.js on your website. -->
<script src="https://js.stripe.com/v3"></script>

<!-- Create a button that your customers click to complete their purchase. Customize the styling to suit your branding. -->
<button
  style="background-color:#6772E5;color:#FFF;padding:8px 12px;border:0;border-radius:4px;font-size:1em"
  id="checkout-button-plan_EvEVdQy8YYKXRQ"
  role="link"
>
  Subscribe to Single Property Edition. Cancel anytime.
</button>

<div id="error-message"></div>

<script>
  var stripe = Stripe('pk_live_tAbLocuhkyEjZbaTdIa30Nuq');

  var checkoutButton = document.getElementById('checkout-button-plan_EvEVdQy8YYKXRQ');
  checkoutButton.addEventListener('click', function () {
    // When the customer clicks on the button, redirect
    // them to Checkout.
    stripe.redirectToCheckout({
      items: [{plan: 'plan_EvEVdQy8YYKXRQ', quantity: 1}],

      // Note that it is not guaranteed your customers will be redirected to this
      // URL *100%* of the time, it's possible that they could e.g. close the
      // tab between form submission and the redirect.
      successUrl: window.location.protocol + '//RiffBiz.com/success',
      cancelUrl: window.location.protocol + '//RiffBiz.com/canceled',
    })
    .then(function (result) {
      if (result.error) {
        // If `redirectToCheckout` fails due to a browser or network
        // error, display the localized error message to your customer.
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
</script>
    - description: >-
        COMING SOON.  Take your analysis to the next level with multiple
        property comparisons.
      items:
        - ''
      plan: Multi Property Edition
      price: '100'
    - description: >-
        COMING SOON.  For the serious investor that wants to understand the
        impact of different assumptions and compare scenarios and properties. 
      items:
        - ''
      plan: Multi Scenario Edition
      price: '500'
---

