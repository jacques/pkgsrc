# $NetBSD: Makefile,v 1.10 2016/06/08 19:23:49 wiz Exp $
#

DISTNAME=	Padre-Plugin-DataWalker-0.02
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	7
CATEGORIES=	editors perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=Padre/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://search.cpan.org/dist/Padre-Plugin-DataWalker/
COMMENT=	Simple Perl data structure browser Padre
LICENSE=	${PERL5_LICENSE}

MAKE_JOBS_SAFE=	no

DEPENDS+=	p5-Padre>=0.47:../../editors/p5-Padre
DEPENDS+=	p5-Wx-Perl-DataWalker>=0.02:../../devel/p5-Wx-Perl-DataWalker
DEPENDS+=	p5-YAML-LibYAML-[0-9]*:../../textproc/p5-YAML-LibYAML

BUILD_DEPENDS+=	p5-Locale-Msgfmt>=0.14:../../devel/p5-Locale-Msgfmt

PERL5_PACKLIST=		auto/Padre/Plugin/DataWalker/.packlist
PERL5_MODULE_TYPE=	Module::Install::Bundled

#pre-configure:
#	cd ${WRKSRC} && find `pwd` -name "*.orig" -type f | xargs rm

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
