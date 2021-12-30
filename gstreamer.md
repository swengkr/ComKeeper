gst-launch-1.0 gdiscreencapsrc cursor=TRUE monitor=1 ! videorate ! "video/x-raw,framerate=10/1" ! videoscale ! video/x-raw,width=640,height=480 ! videoconvert ! autovideosink sync=false

1) gdiscreencapsrc : 윈도우 화면을 캡처한다. cursor 속성은 커서 포함 유무이고, monitor 속성은 다중 모니터일 때 그 인덱스를 나타낸다.
2) videorate : 프레임레이트를 설정한다.
3) videoscale : 이미지 크기를 설정한다.
4) videoconvert : 비디오 형식을 변환한다.
5) autovideosink : 캡처된 비디오를 랜더링한다. sync 속성은 비동기로 설정한다.
