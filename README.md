## StudentVue Mock Server

<p align="center"><img src="https://github.com/StudentVue-Community/MockServer/raw/master/demos/output.gif" width="200"></p>

This is a in-progress implementation of a server that functions like the backend of the StudentVue app, the API of which is partially documented [here](https://github.com/StudentVue-Community/SOAPI-Docs).

So far, it only supports some background methods and StudentVue messages.

Currently, I'm hosting an instance at [studentvue1.kaijchang.com](https://studentvue1.kaijchang.com/), but the uptime might be flaky.

## Running an Instance

You'll need a SSL certificate for your server and port forwarding for ports 80 and 443.

After you've done so, you can run your instance like so:

`CERT="<PATH TO CERTIFICATE>" KEY="<PATH TO PRIVATE KEY>" ORIGIN="<FRONT FACING URL>" yarn start`

For me, this command looks like `CERT="/etc/letsencrypt/live/studentvue1.kaijchang.com/fullchain.pem" KEY="/etc/letsencrypt/live/studentvue1.kaijchang.com/privkey.pem" ORIGIN="https://studentvue1.kaijchang.com" yarn start`

After that, you should be able to interface to this server similarly to any official server for StudentVue.
