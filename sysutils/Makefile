COMMENT =	FUSE-based webdav filesystem

DISTNAME =	wdfs-1.4.2
PKGNAME =	${DISTNAME:S/-/-fuse-/}

CATEGORIES =	sysutils

HOMEPAGE =	http://noedler.de/projekte/wdfs/

# GPLv2
PERMIT_PACKAGE =	Yes

WANTLIB += c fuse glib-2.0 intl neon pthread

MASTER_SITES =	${HOMEPAGE}

LIB_DEPENDS =	devel/glib2 \
		net/neon

CONFIGURE_STYLE =	gnu
CONFIGURE_ENV =	LDFLAGS=-pthread

.include <bsd.port.mk>
