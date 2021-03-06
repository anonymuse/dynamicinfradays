---
title: Event
menu: Event
buttons:
    - text: Get your ticket!
      url: http://dynamicinfradays.org/events/2016-nyc/sign-up/
      primary: true
---

# ContainerDays NYC 2016

The community container and dynamic infrastructure (un)conference returns to NYC for a second edition: November 3-4, 2016.

#### Learn, share, experiment

##### Looking to learn how to go from Container 101 to doing this 'for real'? What the technical story is behind containers? What it's like to run Docker, Kubernetes, Mesos, etc. in production? Where the experts see this technology going..?

### Mark your calendars: **November 3-4, 2016**

----

## What is ContainerDays NYC?

ContainerDays NYC is a community (un)conference to encourage discussion and learning on the subject of containers and dynamic infrastructure generally. The [programme](#programme) is a mix of talks, workshops and OpenSpaces sessions by users, contributors and extenders from all corners of the space.

Whether you're an expert or new to the space, there'll be plenty for you to learn and discuss. It's an (un)conference, so _you_ get to pick many of the topics!

<script>
// eventPage
var eventPage = 'https://www.eventbrite.com/e/containerdays-nyc-2016-tickets-26650870471';

// regex to grab tickets remaining element
var reg = /(\d+)(\sTickets?)/;

// default to this ticket amount, used when event doesn't report ticket counts
var tr = 'tickets';

// do the thing
$.get('https://crossorigin.me/' + eventPage)
  .success(function(data) {
    text = $('td[id="remaining_quant_52596311_None"]', data).text();
    hasWaitlist = /Add to Waitlist/.exec(data);
    console.log('DEBUG: Has waitlist? ' + hasWaitlist);
    try {
      tr = reg.exec(text)[1];
      $('.button.primary').html('Get your ticket - ' + tr + ' remaining');
      console.log('Successfully updated sign-up button');
    } catch (err) {
      console.log('No tickets available');
      if (hasWaitlist) {
        msg = 'Get on the waitlist';
      } else {
        msg = 'Sold out';
      }
      $('.button.primary').html(msg);
    }
  })
  .error(function(jqXHR, textStatus, errorThrown) {
    console.log('Failed to get ticket count');
  });
</script>