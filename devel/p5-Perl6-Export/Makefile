# $NetBSD: Makefile,v 1.19 2021/05/24 19:51:24 wiz Exp $
#

DISTNAME=	Perl6-Export-0.009
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	5
CATEGORIES=	devel perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=../../authors/id/D/DC/DCONWAY/}

MAINTAINER=	abs@absd.org
HOMEPAGE=	https://metacpan.org/release/Perl6-Export
COMMENT=	Implements the Perl 6 'is export(...)' trait
LICENSE=	${PERL5_LICENSE}

USE_LANGUAGES=	# empty
PERL5_PACKLIST=	auto/Perl6/Export/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
