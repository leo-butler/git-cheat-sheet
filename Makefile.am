all: info html

info: git-cheat-sheet.info

git-cheat-sheet.info : git-cheat-sheet.texi
	makeinfo --force git-cheat-sheet.texi

html: git-cheat-sheet.html

git-cheat-sheet.html: git-cheat-sheet.texi
	makeinfo --force --html git-cheat-sheet.texi

include $(top_srcdir)/common.mk
genericdir = $(dochtmldir)

htmlname = git-cheat-sheet
htmlinstdir = $(dochtmldir)
include $(top_srcdir)/common-html.mk

clean-local: clean-info
clean-local: clean-html

clean-info:
	rm -f git-cheat-sheet.info*

clean-html:
	rm -fr git-cheat-sheet

