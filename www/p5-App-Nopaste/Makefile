# $NetBSD: Makefile,v 1.25 2016/06/08 19:24:55 wiz Exp $

DISTNAME=	App-Nopaste-1.004
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	2
CATEGORIES=	www perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=App/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://search.cpan.org/dist/App-Nopaste/
COMMENT=	Perl 5 module providing easy access to any pastebin
LICENSE=	${PERL5_LICENSE}

USE_LANGUAGES=	# empty
PERL5_PACKLIST= auto/App/Nopaste/.packlist

REPLACE_PERL+=	script/nopaste

DEPENDS+=	p5-Moose>=0.74:../../devel/p5-Moose
DEPENDS+=	p5-MooseX-Getopt>=0.17:../../devel/p5-MooseX-Getopt
DEPENDS+=	p5-WWW-Mechanize-[0-9]*:../../www/p5-WWW-Mechanize

# Recommended dependencies
DEPENDS+=	p5-Clipboard-[0-9]*:../../x11/p5-Clipboard
DEPENDS+=	p5-Config-INI-[0-9]*:../../devel/p5-Config-INI
DEPENDS+=	p5-WWW-Pastebin-PastebinCom-Create-[0-9]*:../../www/p5-WWW-Pastebin-PastebinCom-Create
#DEPENDS+=	{perl>=5.6.1,p5-File-Temp-[0-9]*}:../../devel/p5-File-Temp

# for make test
BUILD_DEPENDS+=	p5-JSON-MaybeXS-[0-9]*:../../converters/p5-JSON-MaybeXS
BUILD_DEPENDS+=	p5-Module-Pluggable-[0-9]*:../../devel/p5-Module-Pluggable
BUILD_DEPENDS+=	p5-Test-Deep-[0-9]*:../../devel/p5-Test-Deep

PERL5_MODULE_TYPE=	Module::Install::Bundled

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
