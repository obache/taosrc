# $NetBSD: Makefile,v 1.37 2020/08/17 20:19:18 leot Exp $
#

DISTNAME=		scim-sinhala-0.1.0
PKGREVISION=		33
CATEGORIES=		inputmethod
MASTER_SITES=		${MASTER_SITE_OSDN:=scim-imengine/16666/}

MAINTAINER=		pkgsrc-users@NetBSD.org
HOMEPAGE=		http://osdn.jp/projects/scim-imengine/
COMMENT=		SCIM IMEngine module for Sinhala
LICENSE=		gnu-gpl-v2

USE_LANGUAGES=		c c++
USE_PKGLOCALEDIR=	yes
USE_LIBTOOL=		yes
USE_TOOLS+=		msgfmt pkg-config
GNU_CONFIGURE=		yes

.include "../../devel/gettext-lib/buildlink3.mk"
.include "../../inputmethod/scim/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
