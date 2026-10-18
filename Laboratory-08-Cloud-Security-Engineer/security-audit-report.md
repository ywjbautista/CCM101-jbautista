
# Security Audit Report

## 1. Principle of Least Privilege (PoLP)

The Principle of Least Privilege means that users and services should receive only the permissions necessary to perform their tasks. This helps prevent unnecessary access to sensitive resources and limits potential damage if an account is compromised.

## 2. Attack Surface

The attack surface of a virtual machine includes the points where an attacker might attempt to access or affect the system. Examples include open network ports, running services, and exposed applications. Reducing unnecessary services and ports helps lower the system's exposure to attacks.

## 3. Default Deny Policy

A Default Deny policy blocks incoming traffic unless a firewall rule explicitly permits it. This is safer because unauthorized connections are blocked by default instead of relying on individual rules to identify every possible attacker.
