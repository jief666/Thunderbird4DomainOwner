# Thunderbird for Domain Owner
Patch to be able to send email using any address from your internet domain.

### What does this do?
With this patch:
- when you'll compose a new message, you'll be able to edit the "from" field. You can replace the local_part of the email address by anything.
- when you reply or forward, Thunderbird will detect the address where you received the email and use it as the 'From' address.

##Why?
When you own an internet domain, you can send and receive email using anything before the @. All these email will arrive in the same inbox but with a different "from" address.
If you reply or forward, Thunderbird will use your configured email address, rather than the one the message was sent to.

Without this patch, you'd have to create an account for all the email address you'd like to use on your domain.

##How to build

If you don't know how to build Thunderbird, a possibility is to take a look at my other project : [https://github.com/jief666/Building-Thunderbird](https://github.com/jief666/Building-Thunderbird) (switch to a branch according to the Thunderbird version).
This project will install everthing, include brew, in a folder.
You can put the patch file in the dev folder and rename it pacthes.txt, it'll be applied automatically when the Thunderbird sources are untared.