# Stripe Payment Demo

1. [Introduction](#introduction)
2. [Requirements](#requirements)
4. [Configuration](#configuration)
5. [Usage](#usage)

## Introduction

This is a demo application for Stripe payment integration. It is built with Laravel 5.5 and Vue.js 2.5. It uses Stripe's Elements to create a payment form and Stripe's Checkout to create a checkout form.

## Requirements

### for server
- python 3.9 or higher
- flask
- stripe

### for mobile
- android
- dependencies
    ```
    implementation 'com.stripe:stripe-android:20.21.1'
    implementation 'com.github.kittinunf.fuel:fuel:2.3.1'
    implementation 'com.github.kittinunf.fuel:fuel-json:2.3.1'
    ```
- Stripe account (in test mode)
- databinding enabled
- Internet permission

## Configuration
1. Run the flask server
    ```
    python server.py
    ```
2. Change the server url in the android app in strings.xml
    ```
    <string name="server_url">http://xxx.xxx.xxx.xxx:port</string>
    ```
3. Change the stripe publishable key in the android app in strings.xml
    ```
    <string name="stripe_publishable_key">pk_test_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</string>
    ```
4. Change the stripe secret key and publisable_key in the server.py
    ```
    pKey='pk...'
    sKey='sk...'
    ```
5. Run android app

