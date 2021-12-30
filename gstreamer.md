gst-launch-1.0 gdiscreencapsrc cursor=TRUE monitor=1 ! videorate ! "video/x-raw,framerate=10/1" ! videoscale ! video/x-raw,width=640,height=480 ! videoconvert ! autovideosink sync=false
