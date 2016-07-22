*******************************
Building and Deploying MEDIator
*******************************

Setting the Environment Variables
#################################

Set the API_KEY, MASHAPE_AUTHORIZATION, and BASE_UR as environment variables.

For example, in Linux.

    export API_KEY=your-api-key

    export MASHAPE_AUTHORIZATION=your-mashape-authorization

    export BASE_URL=services.cancerimagingarchive.net/services/v4/TCIA/query


Building and Executing Using Apache Maven 3.x.x
###############################################

mvn package

It is expected to have the TCIA API_KEY set in the environment variables to build with tests.


If you do not have a TCIA API_KEY yet, please build with skipping the tests.

mvn package -DskipTests
