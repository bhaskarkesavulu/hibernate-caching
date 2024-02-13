
WARN: HHH020007: read-only cache configured for mutable entity [com.cache.hibernate.Employee]
Feb 13, 2024 4:58:37 PM org.hibernate.resource.transaction.backend.jdbc.internal.DdlTransactionIsolatorNonJtaImpl getIsolatedConnection
INFO: HHH10001501: Connection obtained from JdbcConnectionAccess [org.hibernate.engine.jdbc.env.internal.JdbcEnvironmentInitiator$ConnectionProviderJdbcConnectionAccess@6c000e0c] for (non-JTA) DDL execution was not in auto-commit mode; the Connection 'local transaction' will be committed and the Connection will be set into auto-commit mode.
Hibernate: select employee0_.id as id1_0_0_, employee0_.name as name2_0_0_, employee0_.salary as salary3_0_0_ from employee employee0_ where employee0_.id=?

1 Bhaskar 80000

1 Bhaskar 80000

If you see Hibernate didn't fired query for 2nd result because of cache magic
