all:
	@gcc -g -Wall -D_GNU_SOURCE rzscontrol.c -o rzscontrol -I ../include -I../..

doc:
	@xmllint --noout --valid man/rzscontrol.xml
	@xsltproc -o man/ /usr/share/kde4/apps/ksgmltools2/docbook/xsl/manpages/docbook.xsl \
		man/rzscontrol.xml
	@man2html man/rzscontrol.1 > man/rzscontrol.html

clean:
	@rm -rf rzscontrol
#	@rm -rf man/rzscontrol.1
