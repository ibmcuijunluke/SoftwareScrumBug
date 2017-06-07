# SoftwareScrumBug
JIRA JSQL
project = SAAS AND issuetype = Bug AND issuetype != 需求（慧云） AND status in (Open, Reopened, Fixing, Resolve) AND component in (EMPTY, AR-应收, CMM-共同参数, CRM-个人法人, CRS-中央Order, FIN-收银, HK-客房, POS-餐饮, RPT-报表, RSV-预订) AND BUG等级 = 1级 OR 慧云BUG等级 = 紧急 AND issuetype != 需求（慧云） AND created >= -5d ORDER BY summary ASC, priority DESC, updated DESC

project = SAAS AND issuetype = Bug AND issuetype != 需求（慧云） AND status in (Open, Reopened, Fixing, Resolve) AND component in (EMPTY, AR-应收, CMM-共同参数, CRM-个人法人, CRS-中央Order, FIN-收银, HK-客房, POS-餐饮, RPT-报表, RSV-预订) AND BUG等级 in (1级, 2级, 3级, 4级, 5级) OR 慧云BUG等级 in (紧急, 普通) AND issuetype != 需求（慧云） AND created <= -5d ORDER BY summary ASC, priority DESC, updated DESC

project = SAAS AND issuetype = Bug AND issuetype != 需求（慧云） AND status in (Open, Reopened, Fixing, Resolve) AND component in (EMPTY, AR-应收, CMM-共同参数, CRM-个人法人, CRS-中央Order, FIN-收银, HK-客房, POS-餐饮, RPT-报表, RSV-预订) AND BUG等级 in (2级, 3级, 4级, 5级) OR 慧云BUG等级 = 普通 AND issuetype != 需求（慧云） AND created >= -5d ORDER BY summary ASC, priority DESC, updated DESC

#####################################################################

project = SAAS AND issuetype = Bug AND issuetype != 需求（慧云） AND status in (Open, Reopened, Fixing, Resolve) AND component in (EMPTY, AR-应收, CMM-共同参数, CRM-个人法人, CRS-中央Order, FIN-收银, HK-客房, POS-餐饮, RPT-报表, RSV-预订) AND (BUG等级 = 1级 OR 慧云BUG等级 = 紧急) ORDER BY summary ASC, priority DESC, updated DESC



project = SAAS AND issuetype in (Bug, 需求（慧云）) AND status in (Open, Reopened, Fixing, DelayResolved, Resolve) AND component in (EMPTY, AR-应收, CMM-共同参数, CRM-个人法人, CRS-中央Order, FIN-收银, HK-客房, POS-餐饮, RPT-报表, RSV-预订) AND created >= -7d ORDER BY summary ASC, priority DESC, updated DESC

project = SAAS AND issuetype = Bug AND status in (Open, Reopened, Fixing, Resolve) AND component in (EMPTY, AR-应收, CMM-共同参数, CRM-个人法人, CRS-中央Order, FIN-收银, HK-客房, POS-餐饮, RPT-报表, RSV-预订) AND BUG等级 = 1级 AND created >= -7d ORDER BY summary ASC, assignee DESC, priority DESC, updated DESC
