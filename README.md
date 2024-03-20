# Infrastructure as Code (IaC) Automation with Ansible Automation Platform 2.x+ and F5 Virtual Platform Products

## About
This code was designed for deploying F5 Virtual Platform Products (Big-IP, Distributed Cloud CEs, BIG-IP Next) with Ansible Automation Platform 2.x+ and pre-built execution environments.  The idea is that customers can deploy F5 products with Ansible Automation with ease and the code can be utilized as a framework for building environments in your hybrid or multi-cloud. 

This code is specifically aimed for IaC with Ansible Automation Platform 2.x+ and VMware vSphere, this is something i have been working on for over a year, and still find customers who utilize VMware vSphere as their primary on-prem datacenter.  I hopefully will work on IaC coding for other platforms down the line and expand this code to work with it. 

## Requirements
We utilize the following Execution Engine to deploy this code with Ansible Automation Platform 2.x+, this removes a lot of the problems with dependencies and versioning as the EE is updated with the build and versions that are necessary to run this correctly.

The Execution Enviroment used/tested is located at - quay.io/f5_business_development/day0-ee:latest	

I will eventually update my github repo to continue updating this build via Github + Workflows + Quay but that will be something for down the road. 

## Installation
Just make sure Ansible Automation Platform has the execution environment above added to it and a project with template for the main git repo setup to utilize the code. 

## Use Cases
Infrastructure as Code (IaC) having customers being able to deploy out F5 Virtual Platforms from OVA into vSphere environments with minimal need to do GUI setups and implementations is the primary Use Case.

There are other ROLES in code created for other projects that might expand this code so they are left in for now.

## Testing
This has been tested in multiple lab environments running vSphere 7x and 8x and Ansible Automation Platform (AAP) 2.4+ versions with the above execution environment.   Make sure to look at the vars-examples folder to add the extra variables and ensure you have created credentials in AAP for vSphere connectivity as well as network credentials for accessing the BIG-IP. 
