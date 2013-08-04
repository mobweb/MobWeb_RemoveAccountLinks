# MobWeb_RemoveAccountLinks extension for Magento

Use this extension to remove links from the "My Account" section in the Magento frontend. Usable directly via XML.

## Installation

Install using [colinmollenhour/modman](https://github.com/colinmollenhour/modman/).

## Example Usage

In local.xml:

```
	<?xml version="1.0"?>
	<layout version="0.1.0">
	    <customer_account>
	        <reference name="customer_account_navigation" >
	            <action method="removeLinkByName"><name>recurring_profiles</name></action>
	            <action method="removeLinkByName"><name>billing_agreements</name></action>
	            <action method="removeLinkByName"><name>OAuth Customer Tokens</name></action>
	        </reference>
	    </customer_account>
	</layout>
```

## Questions? Need help?

Most of my repositories posted here are projects created for customization requests for clients, so they probably aren't very well documented and the code isn't always 100% flexible. If you have a question or are confused about how something is supposed to work, feel free to get in touch and I'll try and help: [info@mobweb.ch](mailto:info@mobweb.ch).