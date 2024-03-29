# SolidusFulfillmentEmails

An extension for solidus that makes it possible to create custom emails for each product when an order is finalized.

## Installation

Add this gem to your Gemfile

```
gem 'solidus_fulfillment_emails', github: 'byteable-dev/solidus_fulfillment_emails', tag: '1.0.0'
```

Then run bundle install

```
bundle install
```

And then install migrations and setup the payment method

```
rails solidus_fulfillment_emails:install:migrations
rake db:migrate
```

## Replacements

You can use the following replacements in your email templates:

| Replacement      | Description |
|------------------| ----------- |
| {{order_number}} | The order number |
| {{order_total}}  | The total of the order |
 | {{name}}         | The name of the customer |
