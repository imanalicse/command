bin\cake cache clear_all

#### Create migration:
bin\cake bake migration CreateAfterPayPaymentsTable

bin\cake bake migration AddPaymentMethodDisplayNameToOrders

#### Run Migration:
bin\cake migrations migrate

#### Create Seeder:
bin\cake bake seed UpdateOldOrganisationPaymentMethods

#### Run Seed:
bin\cake migrations seed --seed ActivitiesFeedSeed

#### migration database
SELECT * from phinxlog WHERE migration_name='AddIsLastItemCompletedColumnToSurveyQuestionAnswers';

DELETE FROM `phinxlog` WHERE migration_name = 'CreateAfterPayPaymentsTable'