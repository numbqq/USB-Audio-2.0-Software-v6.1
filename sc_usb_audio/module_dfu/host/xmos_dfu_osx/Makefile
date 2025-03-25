all:
	g++ -g -o tone_dfu_tool.x86_64 xmosdfu.cpp -I. -IOSX libusb-1.0.0-x86_64.dylib -m64 -target x86_64-apple-macos10.12
	g++ -g -o tone_dfu_tool.arm64 xmosdfu.cpp -I. -IOSX libusb-1.0.0-arm64.dylib -m64 -target arm64-apple-macos11
	lipo -create -output tone_dfu_tool tone_dfu_tool.x86_64 tone_dfu_tool.arm64

clean:
	rm -rf tone_dfu_tool tone_dfu_tool.*
