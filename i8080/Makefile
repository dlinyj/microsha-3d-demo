all: generate build

IMAGE= microsha_demo

build:
	zasm --asm8080 -l $(IMAGE).lst $(IMAGE).asm

clean:
	-rm $(IMAGE).hex $(IMAGE).bin $(IMAGE).lst frames.asm
	$(MAKE) -C generator clean

generate:
	$(MAKE) -C generator
	cp generator/frames.asm .



