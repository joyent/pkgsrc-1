# $NetBSD: Makefile,v 1.23 2021/05/24 19:51:52 wiz Exp $

DISTNAME=	Throwable-0.200013
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	6
CATEGORIES=	devel perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=../../authors/id/R/RJ/RJBS/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://metacpan.org/release/Throwable
COMMENT=	Perl 5 role for classes that can be thrown
LICENSE=	${PERL5_LICENSE}

DEPENDS+=	p5-Devel-StackTrace>=1.2100:../../devel/p5-Devel-StackTrace
DEPENDS+=	p5-Moo>=1.000001:../../devel/p5-Moo

PERL5_PACKLIST=		auto/Throwable/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
