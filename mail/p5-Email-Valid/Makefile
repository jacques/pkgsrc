# $NetBSD: Makefile,v 1.39 2016/06/08 19:23:57 wiz Exp $

DISTNAME=		Email-Valid-1.200
PKGNAME=		p5-${DISTNAME}
PKGREVISION=		1
CATEGORIES=		mail perl5
MASTER_SITES=		${MASTER_SITE_PERL_CPAN:=Email/}

MAINTAINER=		pkgsrc-users@NetBSD.org
HOMEPAGE=		http://search.cpan.org/dist/Email-Valid/
COMMENT=		Perl5 module for testing validity of an email address
LICENSE=		${PERL5_LICENSE}

DEPENDS+=		p5-MailTools-[0-9]*:../../mail/p5-MailTools
DEPENDS+=		p5-Net-DNS-[0-9]*:../../net/p5-Net-DNS
DEPENDS+=		p5-Net-Domain-TLD-[0-9]*:../../net/p5-Net-Domain-TLD
DEPENDS+=		p5-IO-CaptureOutput-[0-9]*:../../devel/p5-IO-CaptureOutput

PERL5_PACKLIST=		auto/Email/Valid/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
