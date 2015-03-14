# $FreeBSD$

PORTNAME=	cxtracker
DISTVERSION= ${GH_COMMIT}
CATEGORIES=	security
DISTFILES=	shadowbq-cxtracker-0.9.9.0-ga6c7e26.tar.gz

MAINTAINER=	shadowbq@gmail.com
COMMENT=	Network sniffer that generates IPFIX type logs

LICENSE=	GPLv2

USE_GITHUB=	yes
GH_ACCOUNT=	shadowbq
GH_PROJECT=	cxtracker
GH_TAG=		${GH_COMMIT}
GH_COMMIT=	6e0bd73

SUB_FILES=	pkg-message

USES=		gmake

USE_RC_SUBR=	cxtracker

.include <bsd.port.options.mk>

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/src/bin/cxtracker \
		${STAGEDIR}${PREFIX}/bin
	${MKDIR} ${STAGEDIR}/var/db/cxtracker

.include <bsd.port.mk>
