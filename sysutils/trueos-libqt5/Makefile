# $FreeBSD$

PORTNAME=	trueos-libqt5
PORTVERSION=	20171003
CATEGORIES=	sysutils

MAINTAINER=	jt@ixsystems.com
COMMENT=	TrueOS QT5 Library

LICENSE=	BSD2CLAUSE

ONLY_FOR_ARCHS=	amd64

WRKSRC_SUBDIR=	src-qt5
MAKE_ARGS=	PREFIX=${STAGEDIR}${PREFIX}

MAKE_JOBS_UNSAFE=	yes

USES=		qmake shebangfix tar:xz
USE_LDCONFIG=	yes
USE_QT5=	core gui network svg linguist \
		buildtools x11extras widgets
USE_GL+=	gl

WRKSRC_SUBDIR=	src-qt5

QMAKE_ARGS=	CONFIG+="configure"

USE_GITHUB=	yes
GH_ACCOUNT=	trueos
GH_PROJECT=	trueos-libqt5
GH_TAGNAME=	9e92b465d823185c9b96f2017e06f2a06b6143fa

.include <bsd.port.mk>
