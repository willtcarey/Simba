.PHONY:    default clean tarball

core = client ocr

all:
#	@python docgen.py `echo $(core) | sed -r \
#        's/(\w+)/..\/Units\/MMLCore\/\1.pas/g'` > /dev/null
	@make -C Pics/
	@make -C sphinx/ singlehtml latexpdf

clean:
#	@rm -f `echo $(core) | sed -r 's/(\w+)/sphinx\/\1.rst/g'`
	@make -C Pics/ clean
	@make -C sphinx/ clean

tarball:
	@$(MAKE) all
#	@tar cjf doc.tar.bz2 -C sphinx/_build/ html
