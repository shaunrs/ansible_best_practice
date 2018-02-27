# Ansible Tips and Tricks

## Role structure
### Reusable Code

## Inventory structure

## Variable Precedence

## Modules - When, how and why
 
## Using Python 2 on newer OS

## Addressing Scale
### Fail Fast on remote connections
It is often useful to have long timeouts and/or many retries when talking to a large number of servers, especially when they are geographically dispersed.

This often introduces unwanted delays on detecting unreachable servers during playbook runs.

To address this, we can setup some initial tasks to verify reachability.

These will:
1. Ensure the SSH port is listening, and has OpenSSH running
1. Ensure we can SSH into the server using our credentials

The timeout for these tasks can be set relatively shorter.

See the [example here](examples/fail-fast.yml).

## Testing
