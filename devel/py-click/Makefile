# $NetBSD: Makefile,v 1.10 2016/04/13 17:58:32 wiz Exp $

DISTNAME=	click-6.6
PKGNAME=	${PYPKGPREFIX}-${DISTNAME}
CATEGORIES=	devel
MASTER_SITES=	${MASTER_SITE_PYPI:=c/click/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://pypi.python.org/pypi/click
COMMENT=	Simple wrapper around optparse for powerful command line utilities
LICENSE=	modified-bsd

BUILD_DEPENDS+=	${PYPKGPREFIX}-test-[0-9]*:../../devel/py-test

USE_LANGUAGES=	# none

do-test:
	cd ${WRKSRC}/tests && PYTHONPATH=.. py.test-${PYVERSSUFFIX} --tb=short

.include "../../lang/python/egg.mk"
.include "../../mk/bsd.pkg.mk"
