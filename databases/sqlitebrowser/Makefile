# $NetBSD: Makefile,v 1.20 2016/04/11 19:01:46 ryoon Exp $

DISTNAME=	sqlitebrowser-3.8.0
PKGREVISION=	2
CATEGORIES=	databases x11
MASTER_SITES=	${MASTER_SITE_GITHUB:=sqlitebrowser/}
GITHUB_PROJECT=	sqlitebrowser
GITHUB_TAG=	v${PKGVERSION_NOREV}

MAINTAINER=	pkgsrc-users@NetBSD.org
COMMENT=	Qt4 lightweight GUI editor/viewer for SQLite Databases
HOMEPAGE=	http://sqlitebrowser.org/
LICENSE=	mpl-2.0 OR gnu-gpl-v3

USE_LANGUAGES=	c c++
USE_CMAKE=	yes

.include "../../databases/sqlite3/buildlink3.mk"
.include "../../x11/qt4-libs/buildlink3.mk"
.include "../../x11/qt4-tools/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
