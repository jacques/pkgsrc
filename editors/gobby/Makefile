# $NetBSD: Makefile,v 1.43 2016/03/10 21:08:43 nros Exp $

DISTNAME=	gobby-0.4.12
PKGREVISION=	25
CATEGORIES=	editors
MASTER_SITES=	http://releases.0x539.de/gobby/

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://gobby.0x539.de/
COMMENT=	Collaborative Editor
LICENSE=	gnu-gpl-v2

USE_LANGUAGES=		c c++
USE_PKGLOCALEDIR=	yes
USE_TOOLS+=		gmake intltool msgfmt pkg-config
GNU_CONFIGURE=		yes

CXXFLAGS+=		-std=c++11

.include "options.mk"

.include "../../devel/glibmm/buildlink3.mk"
.include "../../devel/libsigc++/buildlink3.mk"
.include "../../editors/obby/buildlink3.mk"
.include "../../graphics/hicolor-icon-theme/buildlink3.mk"
.include "../../net/net6/buildlink3.mk"
.include "../../textproc/libxml++/buildlink3.mk"
.include "../../x11/gtkmm/buildlink3.mk"
.include "../../x11/gtksourceview2/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
