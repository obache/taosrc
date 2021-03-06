# $NetBSD: Makefile,v 1.42 2021/05/10 12:47:54 prlw1 Exp $

DISTNAME=	accerciser-3.38.0
PKGREVISION=	2
CATEGORIES=	devel gnome
MASTER_SITES=	${MASTER_SITE_GNOME:=sources/accerciser/${PKGVERSION_NOREV:R}/}
EXTRACT_SUFX=	.tar.xz

MAINTAINER=	prlw1@cam.ac.uk
HOMEPAGE=	https://live.gnome.org/Accerciser/
COMMENT=	Interactive Python accessibility explorer for the GNOME desktop
LICENSE=	modified-bsd

PREV_PKGPATH=	devel/accerciser3

USE_TOOLS+=		gmake itstool msgfmt pkg-config
USE_PKGLOCALEDIR=	yes
GNU_CONFIGURE=		yes
PY_PATCHPLIST=		yes
REPLACE_PYTHON=		plugins/ipython_view.py
REPLACE_PYTHON+=	src/accerciser.in

# msgfmt: unknown option -- desktop
GETTEXT_TOOLS_REQD=	0.19.8

DEPENDS+=	libwnck3-[0-9]*:../../devel/libwnck3
DEPENDS+=	${PYPKGPREFIX}-at-spi2-[0-9]*:../../devel/py-at-spi2
DEPENDS+=	${PYPKGPREFIX}-gobject3-[0-9]*:../../devel/py-gobject3
DEPENDS+=	${PYPKGPREFIX}-ipython>=1.2.1:../../devel/py-ipython
DEPENDS+=	${PYPKGPREFIX}-Xlib-[0-9]*:../../x11/py-Xlib

# dependencies to keep package's configure script happy:
PYTHON_VERSIONS_INCOMPATIBLE=	27

.include "../../x11/gtk3/buildlink3.mk"
.include "../../devel/at-spi2-core/buildlink3.mk"
.include "../../devel/glib2/schemas.mk"
.include "../../devel/py-gobject3-common/buildlink3.mk"
.include "../../graphics/hicolor-icon-theme/buildlink3.mk"
.include "../../lang/python/application.mk"
.include "../../lang/python/extension.mk"
.include "../../sysutils/desktop-file-utils/desktopdb.mk"
.include "../../mk/bsd.pkg.mk"
