# $NetBSD: Makefile,v 1.18 2016/04/05 12:43:23 fhajny Exp $

DISTNAME=	libbson-1.3.5
CATEGORIES=	devel
MASTER_SITES=	${MASTER_SITE_GITHUB:=mongodb/}

MAINTAINER=	filip@joyent.com
HOMEPAGE=	http://github.com/mongodb/libbson/
COMMENT=	BSON utility library
LICENSE=	apache-2.0

GITHUB_RELEASE=	${PKGVERSION_NOREV}

GNU_CONFIGURE=	yes
USE_LANGUAGES=	c c++
USE_LIBTOOL=	yes
USE_TOOLS+=	gmake pkg-config

PKGCONFIG_OVERRIDE+=	src/libbson-1.0.pc.in

INSTALLATION_DIRS+=	${PKGMANDIR}/man3

post-install:
	${INSTALL_MAN} ${WRKSRC}/doc/man/bson_*.3 \
		${DESTDIR}${PREFIX}/${PKGMANDIR}/man3

.include "../../mk/pthread.buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
