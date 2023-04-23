COMMENT=	Qt5-based GUI for SWORD Bible study tool

GH_ACCOUNT = bibletime
GH_PROJECT = bibletime
GH_TAGNAME = v2.11.2
#SUBST_VAR += GH_TAGNAME

V=			2.11.2
DISTNAME=	bibletime-${V}
CATEGORIES=	textproc misc
PKGNAME=	${DISTNAME}
REVISION=	2
HOMEPAGE=	http://bibletime.info/
MAINTAINER=	Corey Stephan <corey.stephan@stthom.edu>
	
#GPL
PERMIT_PACKAGE=	Yes

MODULES += devel/cmake \
	   x11/qt5 \
	   lang/clang

COMPILER = 	base-clang #ports-gcc

BUILD_DEPENDS += devel/cmake \
		 textproc/sword \
		 textproc/clucene

RUN_DEPENDS = 	x11/qt5/qtwebkit \
		textproc/sword 

LIB_DEPENDS += 	x11/qt5/qtbase \
		textproc/clucene

WANTLIB +=	clucene-core Qt5Core

WANTLIB +=	X11 c m ssl

CXXFLAGS += 	-std=c++11
CONFIGURE_ARGS +=	-DCMAKE_PREFIX_PATH=${LOCALBASE}/lib/qt5/cmake/

.include <bsd.port.mk>
