# All-Ireland-Geo-Spatial

## PostgreSQL configuration

ireland.sql defines the tables of a PostgreSQL dump. Database version 12.5. pgdump version 12.6.

The PostGIS and fuzzystrmatch extensions were installed using the following guide, as the PostgreSQL server was running on an Amazon RDS instance.
https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Appendix.PostgreSQL.CommonDBATasks.PostGIS.html

### counties
| id |

### county_names
| county_id | name | lang | source |

### county_polygons
| id | county_id | polygon |

### baronies
| id | county_id |

### barony_names
| barony_id | name | lang | source |

### barony_polygons
| id | barony_id | polygon |

### places
| id | county_id | classification | coords |

### place_names
| place_id | name | lang | source |