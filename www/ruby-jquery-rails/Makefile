# $NetBSD: Makefile,v 1.9 2015/03/13 16:54:35 taca Exp $

DISTNAME=	jquery-rails-3.1.2
CATEGORIES=	www

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://rubygems.org/gems/jquery-rails/
COMMENT=	Rails jQuery support
LICENSE=	mit

DEPENDS+=	${RUBY_RAILTIES_DEPENDS}
DEPENDS+=	${RUBY_PKGPREFIX}-thor>=0.14<2:../../devel/ruby-thor

.include "../../lang/ruby/gem.mk"
.include "../../mk/bsd.pkg.mk"
