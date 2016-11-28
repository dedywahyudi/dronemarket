---
layout: post
title:  "10_Assign_Drone"
date:   2016-11-19 19:41:45 +0700
categories: post
---

<img src="{{ site.github.url }}/images/posts/2016-11-19/10_Assign_Drone.jpg">

### Component Structure

{% highlight js %}
App
│───Header
└───Content
│   └───Breadcrumb
│   └───AssignDrone
│       └───AssignDroneTitle
│       └───AssignDroneInfo
│       └───AssignDroneWizard
│           └───Step1
│           │   └───SelectDroneItem
│           │   └───WizardButton
│           └───Step2
└───Footer
{% endhighlight %}

### Recommended Libraries

* N/A

### PropTypes

{% highlight ruby %}

-- AssignDroneInfo.jsx --
AssignDroneInfo.propTypes = {
  type: PropTypes.string.isRequired,
  deliverydate: PropTypes.string.isRequired,
  pickuplocation: PropTypes.string.isRequired,
  dropoffdeliverylocation: PropTypes.string.isRequired,
  whattodeliver: PropTypes.string.isRequired,
  weight: PropTypes.number.isRequired,
};

-- SelectDroneItem.jsx --
SelectDroneItem.propTypes = {
  photo: PropTypes.string.isRequired,
  title: PropTypes.string.isRequired,
  serialnumber: PropTypes.string.isRequired,
  speed: PropTypes.string.isRequired,
  flighttime: PropTypes.number.isRequired,
  weight: PropTypes.number.isRequired,
};

{% endhighlight %}
