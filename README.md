# 3scale Workshop

This is a subset of the content present in the [DIL-Agile-Integration](https://github.com/RedHat-Middleware-Workshops/dayinthelife-integration), focused on 3sale.

Order the `DIL-Agile-Integration` workshop then run the following command to update the documentation:

    oc set env  dc/tutorial-web-app -n webapp WALKTHROUGH_LOCATIONS=https://github.com/GuilhermeCamposo/workshop_3scale.git

You can also change the image used for the solution explorer, this way project are not created by each lab.

    oc patch dc/tutorial-web-app -n webapp  --patch '{"spec":{"template":{"spec":{"containers":[{"name":"tutorial-web-app","image":"quay.io/gcamposo/tutorial-web-app:1.0.10"}]}}}}'
